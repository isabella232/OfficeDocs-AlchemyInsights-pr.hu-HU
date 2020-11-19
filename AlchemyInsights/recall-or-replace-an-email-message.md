---
title: E-mail-üzenet visszahívása vagy cseréje
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353508"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="02cd9-102">E-mail-üzenet visszahívása vagy cseréje a Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="02cd9-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="02cd9-103">**Csak a szervezet tagjainak küldött üzeneteket lehet visszahívni**.</span><span class="sxs-lookup"><span data-stu-id="02cd9-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="02cd9-104">Ha például az üzenetet Gmail-címre küldte, a program nem tudja visszahívni.</span><span class="sxs-lookup"><span data-stu-id="02cd9-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="02cd9-105">**Csak a PC-ről küldött üzeneteket lehet visszahívni**.</span><span class="sxs-lookup"><span data-stu-id="02cd9-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="02cd9-106">Ha egy felhasználó a Mac Outlookban vagy a webes Outlookban küld üzenetet, nem lehet visszahívni.</span><span class="sxs-lookup"><span data-stu-id="02cd9-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="02cd9-107">Bérlői rendszergazdaként a **PowerShell használatával visszahívhatja az üzeneteket a felhasználók nevében** (további információt az [e-mailek keresése és törlése](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)című témakörben talál).</span><span class="sxs-lookup"><span data-stu-id="02cd9-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="02cd9-108">A felügyeleti központból nem lehet visszahívni az üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="02cd9-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="02cd9-109">További információt az "e-mail-üzenetek keresése és törlése a szervezetben" című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="02cd9-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="02cd9-110">**Elküldött e-mailek visszahívása vagy cseréje**</span><span class="sxs-lookup"><span data-stu-id="02cd9-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="02cd9-111">Az Outlook ablakának bal oldalán található mappa ablaktáblában válassza az elküldött elemek mappát.</span><span class="sxs-lookup"><span data-stu-id="02cd9-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="02cd9-112">Nyissa meg a visszahívni kívánt üzenetet.</span><span class="sxs-lookup"><span data-stu-id="02cd9-112">Open the message that you want to recall.</span></span> <span data-ttu-id="02cd9-113">Az üzenet megnyitásához duplán kell kattintania.</span><span class="sxs-lookup"><span data-stu-id="02cd9-113">You must double-click to open the message.</span></span> <span data-ttu-id="02cd9-114">Ha kijelöli az üzenetet, hogy az olvasóablakban jelenjen meg, ne engedélyezze az üzenet visszahívását.</span><span class="sxs-lookup"><span data-stu-id="02cd9-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="02cd9-115">Az üzenet lapon válassza a **műveletek**  >  **visszahívása ezt az üzenetet** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="02cd9-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="02cd9-116">Válassza az **üzenet olvasatlan példányainak törlése** vagy az **olvasatlan példányok törlése, majd a csere egy új üzenettel** lehetőséget, és válassza **az OK gombot**.</span><span class="sxs-lookup"><span data-stu-id="02cd9-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="02cd9-117">Ha helyettesítő üzenetet küld, írja meg az üzenetet, és válassza a **Küldés** gombot.</span><span class="sxs-lookup"><span data-stu-id="02cd9-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="02cd9-118">Az üzenet visszahívásának sikere vagy kudarca az Outlook címzettek beállításaitól függ.</span><span class="sxs-lookup"><span data-stu-id="02cd9-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="02cd9-119">Ha további információra van szüksége a visszahívás ellenőrzéséről, olvassa el az [elküldött e-mailek visszahívása vagy cseréje](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)című témakört.</span><span class="sxs-lookup"><span data-stu-id="02cd9-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="02cd9-120">Ha meg **_szeretné keresni és törölni szeretné a szervezetében lévő e-maileket_**, akkor a legegyszerűbb, ha Ön globális rendszergazda. Ha nem globális rendszergazda, fiókját fel kell vennie az eDiscovery-kezelő szerepkörcsoport szerepkör-csoportjához vagy a megfelelőségi keresési szerepkörbe.</span><span class="sxs-lookup"><span data-stu-id="02cd9-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="02cd9-121">Üzenetek törléséhez csatlakoznia kell a szervezeti vagy a keresési és törlési felügyeleti szerepkörhöz.</span><span class="sxs-lookup"><span data-stu-id="02cd9-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="02cd9-122">Az e szerepkörökhöz tartozó engedélyeket a [biztonsági & megfelelőségi központban](https://protection.office.com/)lehet kiosztani.</span><span class="sxs-lookup"><span data-stu-id="02cd9-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="02cd9-123">A törlendő üzenet megtalálásához [hozzon létre egy keresési tartalmat](https://docs.microsoft.com/microsoft-365/compliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="02cd9-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="02cd9-124">[Csatlakozás a biztonsági & megfelelőségi központ powershellhez](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="02cd9-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="02cd9-125">Ha MFA-t (többtényezős hitelesítést) használ, olvassa el [a csatlakozás a Microsoft 365 biztonsági & megfelelőségi központ PowerShell a többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)című témakört.</span><span class="sxs-lookup"><span data-stu-id="02cd9-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
