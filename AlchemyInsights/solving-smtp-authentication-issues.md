---
title: SMTP-hitelesítés és -hibaelhárítás engedélyezése
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077653"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="de063-102">SMTP-hitelesítés és -hibaelhárítás engedélyezése</span><span class="sxs-lookup"><span data-stu-id="de063-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="de063-103">Ha egy postaládában szeretné engedélyezni az SMTP-hitelesítést, vagy egy "Az ügyfél nincs hitelesítve", a "Nem sikerült a hitelesítés" vagy az "SmtpClientAuthentication" hibaüzenet jelenik meg az 5.7.57-es vagy az 5.7.3-as vagy 5.7.139-es hibakódnál, amikor egy eszköz vagy alkalmazás Microsoft 365 hitelesítő funkciójával próbál meg továbbítani egy e-mailt, a probléma megoldásához végezze el az alábbi három műveletet:</span><span class="sxs-lookup"><span data-stu-id="de063-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="de063-104">Tiltsa le [az Azure biztonsági alapértelmezett beállítását](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) A biztonsági alapértelmezések engedélyezése beállítást **Nem** **beállításra.**</span><span class="sxs-lookup"><span data-stu-id="de063-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="de063-105">a.</span><span class="sxs-lookup"><span data-stu-id="de063-105">a.</span></span> <span data-ttu-id="de063-106">Jelentkezzen be az Azure Portalba biztonsági rendszergazdaként, feltételes hozzáféréssel rendelkező rendszergazdaként vagy globális rendszergazdaként.</span><span class="sxs-lookup"><span data-stu-id="de063-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="de063-107">b.</span><span class="sxs-lookup"><span data-stu-id="de063-107">b.</span></span> <span data-ttu-id="de063-108">Tallózással keresse Azure Active Directory > **gombra.**</span><span class="sxs-lookup"><span data-stu-id="de063-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="de063-109">c.</span><span class="sxs-lookup"><span data-stu-id="de063-109">c.</span></span> <span data-ttu-id="de063-110">Válassza **a Biztonsági alapértelmezések kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="de063-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="de063-111">d.</span><span class="sxs-lookup"><span data-stu-id="de063-111">d.</span></span> <span data-ttu-id="de063-112">Állítsa **a Biztonsági alapértékek engedélyezése beállítást** **Nemre.**</span><span class="sxs-lookup"><span data-stu-id="de063-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="de063-113">e.</span><span class="sxs-lookup"><span data-stu-id="de063-113">e.</span></span> <span data-ttu-id="de063-114">Válassza a **Mentés** elemet.</span><span class="sxs-lookup"><span data-stu-id="de063-114">Select **Save**.</span></span>

2. <span data-ttu-id="de063-115">[Engedélyezze az ügyféloldali SMTP-beküldést](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) a licencelt postaládában.</span><span class="sxs-lookup"><span data-stu-id="de063-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="de063-116">a.</span><span class="sxs-lookup"><span data-stu-id="de063-116">a.</span></span> <span data-ttu-id="de063-117">A Microsoft 365 Felügyeleti központ válassza az Aktív **felhasználók** lehetőséget, és jelölje ki a felhasználót.</span><span class="sxs-lookup"><span data-stu-id="de063-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="de063-118">b.</span><span class="sxs-lookup"><span data-stu-id="de063-118">b.</span></span> <span data-ttu-id="de063-119">A Levelek lap Levelezési alkalmazások csoportjában **válassza** a **Levelezőalkalmazások kezelése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="de063-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="de063-120">d.</span><span class="sxs-lookup"><span data-stu-id="de063-120">d.</span></span> <span data-ttu-id="de063-121">Győződjön meg **arról, hogy a Hitelesített SMTP** beállítás be van jelölve (engedélyezve).</span><span class="sxs-lookup"><span data-stu-id="de063-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="de063-122">e.</span><span class="sxs-lookup"><span data-stu-id="de063-122">e.</span></span> <span data-ttu-id="de063-123">Válassza a **Módosítások mentése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="de063-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="de063-124">[Tiltsa le a Multi-Factor Authentication (MFA) hitelesítést](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) a licencelt postaládában.</span><span class="sxs-lookup"><span data-stu-id="de063-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="de063-125">a.</span><span class="sxs-lookup"><span data-stu-id="de063-125">a.</span></span> <span data-ttu-id="de063-126">A navigációs Microsoft 365 Felügyeleti központ a bal oldali navigációs menüben válassza **a Felhasználók**  >  **aktív felhasználók elemet.**</span><span class="sxs-lookup"><span data-stu-id="de063-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="de063-127">b.</span><span class="sxs-lookup"><span data-stu-id="de063-127">b.</span></span> <span data-ttu-id="de063-128">Válassza **a Többtényezős hitelesítés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="de063-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="de063-129">c.</span><span class="sxs-lookup"><span data-stu-id="de063-129">c.</span></span> <span data-ttu-id="de063-130">Jelölje ki a felhasználót, és tiltsa le **a Multi-Factor Auth bővítményt.**</span><span class="sxs-lookup"><span data-stu-id="de063-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
