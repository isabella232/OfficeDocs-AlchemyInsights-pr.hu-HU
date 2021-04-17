---
title: Hiányzó e-mailek karanténban
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831736"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="d2bf8-102">Hiányzó e-mailek a karanténban"</span><span class="sxs-lookup"><span data-stu-id="d2bf8-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="d2bf8-103">A rendszergazdák [megtekinthetik, feladhatják vagy törölhetik ezeket az üzeneteket.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="d2bf8-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="d2bf8-104">A Biztonsági és & megnyitásához nyissa meg a következőt: [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="d2bf8-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="d2bf8-105">A karanténlap közvetlen megnyitásához nyissa meg a következőt: [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="d2bf8-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="d2bf8-106">A következő értékek alapján kereshet:</span><span class="sxs-lookup"><span data-stu-id="d2bf8-106">You can search by the following values:</span></span>  

- <span data-ttu-id="d2bf8-107">**Üzenetazonosító:** Az üzenet globálisan egyedi azonosítója.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="d2bf8-108">Ha kijelöl egy üzenetet a  listában, megjelenik  az Üzenetazonosító érték a megjelenő Részletek előgombra kattintva.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="d2bf8-109">A rendszergazdák az [üzenetkövetés](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) segítségével megkeresheti az üzeneteket és a hozzájuk tartozó üzenetazonosítókat.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="d2bf8-110">**Feladó e-mail-címe:** Egyetlen feladó e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="d2bf8-111">**Címzett e-mail-címe:** Egyetlen címzett e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="d2bf8-112">**Tárgy:** Használja az üzenet teljes tárgyát.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="d2bf8-113">A keresés nem megkülönbözteti a kis- és a nagybetűket.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="d2bf8-114">Miután megadta a keresési feltételeket, a Frissítés gombra kattintva ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **szűrheti** a találatokat.  </span><span class="sxs-lookup"><span data-stu-id="d2bf8-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="d2bf8-115">A karanténban lévő üzenetek és fájlok megtekintéséhez és kezeléséhez a következő parancsmagok használhatók:</span><span class="sxs-lookup"><span data-stu-id="d2bf8-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="d2bf8-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2bf8-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="d2bf8-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2bf8-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="d2bf8-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2bf8-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="d2bf8-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Ne feledje, hogy ez a parancsmag csak üzenetekhez használható, a SharePoint Online-hoz, a OneDrive Vállalati verzióhoz vagy a Teamshez nem tartalmaz kártevőfájlokat.</span><span class="sxs-lookup"><span data-stu-id="d2bf8-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="d2bf8-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="d2bf8-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)