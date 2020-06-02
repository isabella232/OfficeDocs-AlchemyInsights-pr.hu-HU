---
title: 1385-Office-365-riasztási szabályzatok
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 05c58bded5ba45aef8ae3bc1d33491e6e0365c18
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502429"
---
# <a name="alert-policies"></a><span data-ttu-id="4aae4-102">Riasztási házirendek</span><span class="sxs-lookup"><span data-stu-id="4aae4-102">Alert policies</span></span>

<span data-ttu-id="4aae4-103">A Microsoft 365 biztonsági & megfelelőségi központ [alapértelmezett riasztási szabályzatokat](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) kínál, amelyek riasztásokat váltanak ki az Office 365 Enterprise vagy Office 365 US Government E1/G1, E3/G3 vagy E5/G5 előfizetéssel rendelkező szervezetek számára.</span><span class="sxs-lookup"><span data-stu-id="4aae4-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="4aae4-104">Ezért a rendszergazdák kaphatnak egy figyelmeztető e-mail értesítést küldött Office365Alerts@microsoft.com egy tárgysor, például "Egy alacsony súlyosságú riasztás: *neve riasztási házirend*".</span><span class="sxs-lookup"><span data-stu-id="4aae4-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="4aae4-105">A rendszer riasztási értesítéseket küld, ha a rendszer riasztásokat indít el a gyakori tevékenységekhez, például amikor a felhasználók:</span><span class="sxs-lookup"><span data-stu-id="4aae4-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="4aae4-106">Hozzon létre olyan beérkezett üzenetekre vonatkozó szabályokat, amelyek továbbítják az e-maileket.</span><span class="sxs-lookup"><span data-stu-id="4aae4-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="4aae4-107">Engedélyek hozzárendelése a postaládájukhoz.</span><span class="sxs-lookup"><span data-stu-id="4aae4-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="4aae4-108">Nagyszámú fájl megosztása vagy törlése a SharePoint fájlmegosztásban.</span><span class="sxs-lookup"><span data-stu-id="4aae4-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="4aae4-109">Elektronikus adatfeltárási keresések létrehozása és keresési eredmények exportálása.</span><span class="sxs-lookup"><span data-stu-id="4aae4-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="4aae4-110">A riasztás áttekintése és az azokkal kapcsolatos cselekvés:</span><span class="sxs-lookup"><span data-stu-id="4aae4-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="4aae4-111">Nyissa meg a [Biztonsági & megfelelőségi központot,](https://protection.office.com) és jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="4aae4-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="4aae4-112">Kattintson **a Riasztások**  >  **megtekintése értesítések elemre.**</span><span class="sxs-lookup"><span data-stu-id="4aae4-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="4aae4-113">Kattintson egy riasztásra a riasztással kapcsolatos információkat tartalmazó úszó paneloldal megjelenítéséhez.</span><span class="sxs-lookup"><span data-stu-id="4aae4-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="4aae4-114">Műveleteket végrehajthat egy riasztáson, például [eltávolíthat egy gyanús beérkezett üzenetekre vonatkozó szabályt.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)</span><span class="sxs-lookup"><span data-stu-id="4aae4-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="4aae4-115">Vagy egyszerűen zárja be a riasztást a **Feloldás** gombra kattintva az alert úszó panel oldalán.</span><span class="sxs-lookup"><span data-stu-id="4aae4-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="4aae4-116">A riasztási házirendek konfigurálásáról és kezeléséről a cikkben olvashat [bővebben.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)</span><span class="sxs-lookup"><span data-stu-id="4aae4-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="4aae4-117">**Fontos:** A Microsoft e-mail értesítéseinek figyelmeztetése soha nem fogja kérni a következőket:</span><span class="sxs-lookup"><span data-stu-id="4aae4-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="4aae4-118">Jelszó megadása</span><span class="sxs-lookup"><span data-stu-id="4aae4-118">Provide a password</span></span>
- <span data-ttu-id="4aae4-119">A fiók biztonsági adatainak ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="4aae4-119">Verify the security details of your account</span></span>
- <span data-ttu-id="4aae4-120">Hitelesítse magát újra</span><span class="sxs-lookup"><span data-stu-id="4aae4-120">Re-authenticate yourself</span></span>

<span data-ttu-id="4aae4-121">Ha ilyen e-mailt kap, azt nem a Microsoft küldte, és adathalászatnak kell tekinteni.</span><span class="sxs-lookup"><span data-stu-id="4aae4-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="4aae4-122">Ha ez megtörténik, kérjük, [jelentse a Microsoftnak.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)</span><span class="sxs-lookup"><span data-stu-id="4aae4-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>