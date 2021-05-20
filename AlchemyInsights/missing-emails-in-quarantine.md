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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539826"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="3b9e0-102">Hiányzó e-mailek a karanténban"</span><span class="sxs-lookup"><span data-stu-id="3b9e0-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="3b9e0-103">A rendszergazdák [megtekinthetik, feladhatják vagy törölhetik ezeket az üzeneteket.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="3b9e0-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="3b9e0-104">A Biztonsági és & megnyitásához nyissa meg a következőt: [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="3b9e0-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="3b9e0-105">A karanténlap közvetlen megnyitásához nyissa meg a következőt: [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="3b9e0-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="3b9e0-106">A következő értékek alapján kereshet:</span><span class="sxs-lookup"><span data-stu-id="3b9e0-106">You can search by the following values:</span></span>  

- <span data-ttu-id="3b9e0-107">**Üzenetazonosító:** Az üzenet globálisan egyedi azonosítója.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="3b9e0-108">Ha kijelöl egy üzenetet a  listában, megjelenik  az Üzenetazonosító érték a megjelenő Részletek előgombra kattintva.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="3b9e0-109">A rendszergazdák az [üzenetkövetés](/microsoft-365/security/office-365-security/message-trace-scc) segítségével megkeresheti az üzeneteket és a hozzájuk tartozó üzenetazonosítókat.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="3b9e0-110">**Feladó e-mail-címe:** Egyetlen feladó e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="3b9e0-111">**Címzett e-mail-címe:** Egyetlen címzett e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="3b9e0-112">**Tárgy:** Használja az üzenet teljes tárgyát.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="3b9e0-113">A keresés nem megkülönbözteti a kis- és a nagybetűket.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="3b9e0-114">Miután megadta a keresési feltételeket, a Frissítés gombra kattintva ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **szűrheti** a találatokat.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="3b9e0-115">A karanténban lévő üzenetek és fájlok megtekintéséhez és kezeléséhez a következő parancsmagok használhatók:</span><span class="sxs-lookup"><span data-stu-id="3b9e0-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="3b9e0-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="3b9e0-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="3b9e0-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="3b9e0-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="3b9e0-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="3b9e0-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="3b9e0-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Ne feledje, hogy ez a parancsmag csak az üzenetekhez érhető el, a Microsoft Defendertől származó kártevőfájlok nem az Office 365 SharePoint Online- vagy SharePoint-, OneDrive Vállalati verzió- vagy Teams.</span><span class="sxs-lookup"><span data-stu-id="3b9e0-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="3b9e0-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="3b9e0-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)