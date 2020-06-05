---
title: Hiányzó e-mailek a karanténban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569231"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="af8c2-102">Hiányzó e-mailek a karanténban"</span><span class="sxs-lookup"><span data-stu-id="af8c2-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="af8c2-103">A rendszergazdák [megtekinthetik, feladhatják vagy törölhetik ezeket az üzeneteket.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="af8c2-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="af8c2-104">A Biztonsági & megfelelőségi központ megnyitásához nyissa meg a [https://protection.office.com](https://protection.office.com/) t.</span><span class="sxs-lookup"><span data-stu-id="af8c2-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="af8c2-105">A Karantén lap közvetlen megnyitásához nyissa meg a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) at.</span><span class="sxs-lookup"><span data-stu-id="af8c2-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="af8c2-106">A következő értékek szerint kereshet:</span><span class="sxs-lookup"><span data-stu-id="af8c2-106">You can search by the following values:</span></span>  

- <span data-ttu-id="af8c2-107">**Üzenetazonosító**: Az üzenet globálisan egyedi azonosítója.</span><span class="sxs-lookup"><span data-stu-id="af8c2-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="af8c2-108">Ha kijelöl egy üzenetet a listában, az **Üzenetazonosító** értéke megjelenik a **megjelenő Részletek** úszó panelen.</span><span class="sxs-lookup"><span data-stu-id="af8c2-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="af8c2-109">A rendszergazdák [az üzenetek nyomon követésével](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) kereshetik meg az üzeneteket és a hozzájuk tartozó Üzenetazonosító-értékeket.</span><span class="sxs-lookup"><span data-stu-id="af8c2-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="af8c2-110">**Feladó e-mail címe**: Egyetlen feladó e-mail címe.</span><span class="sxs-lookup"><span data-stu-id="af8c2-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="af8c2-111">**Címzett e-mail címe**: Egyetlen címzett e-mail címe.</span><span class="sxs-lookup"><span data-stu-id="af8c2-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="af8c2-112">**Tárgy**: Az üzenet teljes témáját használhatja.</span><span class="sxs-lookup"><span data-stu-id="af8c2-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="af8c2-113">A keresés nem a kis- és nagybetűket nem érzékeny.</span><span class="sxs-lookup"><span data-stu-id="af8c2-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="af8c2-114">Miután megadta a keresési feltételeket, kattintson a ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Frissítés gombra,** a Frissítés gombra az eredmények szűréséhez.  </span><span class="sxs-lookup"><span data-stu-id="af8c2-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="af8c2-115">A karanténban lévő üzenetek és fájlok megtekintéséhez és kezeléséhez használt parancsmagok a következők:</span><span class="sxs-lookup"><span data-stu-id="af8c2-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="af8c2-116">Törlés-KaranténÜzenet</span><span class="sxs-lookup"><span data-stu-id="af8c2-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="af8c2-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="af8c2-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="af8c2-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="af8c2-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="af8c2-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Vegye figyelembe, hogy ez a parancsmag csak üzenetekhez készült, a SharePoint Online, a OneDrive Vállalati verzió vagy a Teams ATP-ből származó kártevőfájlokhoz nem.</span><span class="sxs-lookup"><span data-stu-id="af8c2-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="af8c2-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="af8c2-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)