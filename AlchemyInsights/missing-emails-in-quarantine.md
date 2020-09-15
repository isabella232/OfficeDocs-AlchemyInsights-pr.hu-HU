---
title: Hiányzó e-mailek a karanténban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673716"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="a3c10-102">Hiányzó e-mailek a karanténban "</span><span class="sxs-lookup"><span data-stu-id="a3c10-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="a3c10-103">A rendszergazdák [megtekinthetik, felszabadítják vagy törölhetik ezeket az üzeneteket.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="a3c10-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="a3c10-104">Ha meg szeretné nyitni a biztonsági & megfelelőségi központot, lépjen a webhelyre [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="a3c10-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="a3c10-105">A karantén lap közvetlen megnyitásához lépjen a gombra [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="a3c10-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="a3c10-106">A Keresés az alábbi értékek alapján végezhető el:</span><span class="sxs-lookup"><span data-stu-id="a3c10-106">You can search by the following values:</span></span>  

- <span data-ttu-id="a3c10-107">**Üzenet azonosítója**: az üzenet globálisan egyedi azonosítója.</span><span class="sxs-lookup"><span data-stu-id="a3c10-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="a3c10-108">Ha kijelöl egy üzenetet a listában, az  **üzenet azonosítójának**  értéke megjelenik a megjelenő  **részletek**  panelben.</span><span class="sxs-lookup"><span data-stu-id="a3c10-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="a3c10-109">A rendszergazdák az [üzenet nyomon követésével](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) megkereshetik az üzeneteket és a hozzájuk tartozó üzenet-azonosító értékét.</span><span class="sxs-lookup"><span data-stu-id="a3c10-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="a3c10-110">**Feladó e-mail-címe**: egyetlen feladó e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="a3c10-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="a3c10-111">**Címzett e-mail-címe**: egyetlen címzett e-mail-címe.</span><span class="sxs-lookup"><span data-stu-id="a3c10-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="a3c10-112">**Tárgy**: az üzenet teljes tárgyát használja.</span><span class="sxs-lookup"><span data-stu-id="a3c10-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="a3c10-113">A keresés nem megkülönbözteti a kis-és nagybetűket.</span><span class="sxs-lookup"><span data-stu-id="a3c10-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="a3c10-114">Miután beírta a keresési feltételt, az ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** eredmény szűréséhez kattintson a frissítés gombra.  </span><span class="sxs-lookup"><span data-stu-id="a3c10-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="a3c10-115">A karanténba helyezett üzenetek és fájlok megtekintéséhez és kezelésére használt parancsmagok:</span><span class="sxs-lookup"><span data-stu-id="a3c10-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="a3c10-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a3c10-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="a3c10-117">Exportálás – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a3c10-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="a3c10-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a3c10-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="a3c10-119">Előzetes verzió: ne feledje, hogy ez a parancsmag csak a SharePoint Online, a OneDrive vállalati verzió vagy a Teams ATP [-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)származó üzenetekre, nem pedig a malware-fájlokra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="a3c10-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="a3c10-120">Kiadás – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a3c10-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)