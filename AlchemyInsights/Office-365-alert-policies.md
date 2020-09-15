---
title: 1385 – Office-365 – riasztás – házirendek
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664028"
---
# <a name="alert-policies"></a><span data-ttu-id="b5448-102">Riasztási házirendek</span><span class="sxs-lookup"><span data-stu-id="b5448-102">Alert policies</span></span>

<span data-ttu-id="b5448-103">A Microsoft 365 biztonsági & megfelelőségi központja olyan [alapértelmezett riasztási házirendeket](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) biztosít, amelyek az Office 365 Enterprise vagy az Office 365 amerikai kormányzati verziójában az E1/G1, E3/G3 vagy E5/G5 előfizetéssel rendelkező szervezetek számára indítanak riasztásokat.</span><span class="sxs-lookup"><span data-stu-id="b5448-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="b5448-104">Ezért a rendszergazdák értesítést kaphatnak a Office365Alerts@microsoft.com által elküldött értesítő e-mailben, például "alacsony súlyosságú figyelmeztetés: *az értesítési házirend neve*".</span><span class="sxs-lookup"><span data-stu-id="b5448-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="b5448-105">Riasztási értesítéseket küld a rendszer, ha a riasztások általános tevékenységekre (például a felhasználóknak) jönnek elő:</span><span class="sxs-lookup"><span data-stu-id="b5448-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="b5448-106">E-maileket továbbító beérkezett üzenetekre vonatkozó szabályok létrehozása</span><span class="sxs-lookup"><span data-stu-id="b5448-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="b5448-107">Engedélyek hozzárendelése a postaládához.</span><span class="sxs-lookup"><span data-stu-id="b5448-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="b5448-108">Nagy mennyiségű fájl megosztása vagy törlése a SharePoint-fájlmegosztás alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="b5448-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="b5448-109">EDiscovery-kereséseket hozhat létre, és exportálhatja a keresési eredményeket.</span><span class="sxs-lookup"><span data-stu-id="b5448-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="b5448-110">Riasztás véleményezése és elkövetése:</span><span class="sxs-lookup"><span data-stu-id="b5448-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="b5448-111">Nyissa meg a [biztonsági & megfelelőségi központot](https://protection.office.com) , és kattintson a Bejelentkezés gombra.</span><span class="sxs-lookup"><span data-stu-id="b5448-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="b5448-112">Kattintson a **riasztások**  >  **megtekintése**elemre.</span><span class="sxs-lookup"><span data-stu-id="b5448-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="b5448-113">A riasztásra kattintva megjelenítheti a képernyőn megjelenő, a riasztásról tájékoztató lapot.</span><span class="sxs-lookup"><span data-stu-id="b5448-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="b5448-114">Az értesítéseken műveleteket végezhet, például [eltávolíthat egy gyanús beérkezett üzenetekre vonatkozó szabályt](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="b5448-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="b5448-115">Vagy egyszerűen zárja be a riasztást a riasztási pont lapon a **feloldás** gombra kattintva.</span><span class="sxs-lookup"><span data-stu-id="b5448-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="b5448-116">Az értesítési házirendek beállításáról és kezeléséről további információt  [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)talál.</span><span class="sxs-lookup"><span data-stu-id="b5448-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="b5448-117">**Fontos**: a Microsofttól érkező e-mail-értesítések nem kérik, hogy tegye az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="b5448-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="b5448-118">Jelszó megadása</span><span class="sxs-lookup"><span data-stu-id="b5448-118">Provide a password</span></span>
- <span data-ttu-id="b5448-119">A fiók biztonsági adatainak ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="b5448-119">Verify the security details of your account</span></span>
- <span data-ttu-id="b5448-120">Újbóli hitelesítés</span><span class="sxs-lookup"><span data-stu-id="b5448-120">Re-authenticate yourself</span></span>

<span data-ttu-id="b5448-121">Ha e-mail-üzenetet kap, az nem a Microsoft küldte el, és adathalásznak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="b5448-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="b5448-122">Ha ez megtörténik, kérjük, [jelentse be a Microsoftnak](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="b5448-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>