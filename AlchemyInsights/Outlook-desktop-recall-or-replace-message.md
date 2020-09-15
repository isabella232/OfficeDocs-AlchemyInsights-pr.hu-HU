---
title: Az Outlook asztali e-mail-üzenet visszahívása vagy cseréje
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663992"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="7ea96-102">Outlook-üzenet visszahívása vagy cseréje</span><span class="sxs-lookup"><span data-stu-id="7ea96-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="7ea96-103">Rendszergazdaként a **PowerShell segítségével visszahívhatja az üzeneteket a felhasználók nevében**.</span><span class="sxs-lookup"><span data-stu-id="7ea96-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7ea96-104">A felügyeleti központból nem lehet visszahívni az üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="7ea96-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7ea96-105">**Csak a szervezet tagjainak küldött üzeneteket lehet visszahívni**.</span><span class="sxs-lookup"><span data-stu-id="7ea96-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7ea96-106">Ha az üzenetet Gmail-címre küldték, például nem tudja visszahívni.</span><span class="sxs-lookup"><span data-stu-id="7ea96-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7ea96-107">**A számítógépen csak az Outlook 2016-ból küldött üzeneteket lehet visszahívni**.</span><span class="sxs-lookup"><span data-stu-id="7ea96-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7ea96-108">Ha egy felhasználó a Mac Outlookban vagy a webes Outlookban küld üzenetet, nem lehet visszahívni.</span><span class="sxs-lookup"><span data-stu-id="7ea96-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7ea96-109">E-mailek visszahívása vagy cseréje:</span><span class="sxs-lookup"><span data-stu-id="7ea96-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7ea96-110">Az Outlook ablakának bal oldalán található mappa ablaktáblában válassza az elküldött elemek mappát.</span><span class="sxs-lookup"><span data-stu-id="7ea96-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7ea96-111">Kattintson duplán a felidézni kívánt üzenetre a megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="7ea96-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7ea96-112">Válassza az **üzenet** fület, majd a **műveletek**  >  **visszahívása az üzenettel**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7ea96-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7ea96-113">Válassza az **üzenet olvasatlan példányainak törlése** vagy az **olvasatlan példányok törlése, majd a csere egy új üzenettel**lehetőséget, és kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="7ea96-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7ea96-114">Ha helyettesítő üzenetet küld, írja meg az üzenetet, és válassza a **Küldés**gombot.</span><span class="sxs-lookup"><span data-stu-id="7ea96-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7ea96-115">Az üzenet visszahívásának sikere vagy kudarca az Outlook címzett beállításaitól függ.</span><span class="sxs-lookup"><span data-stu-id="7ea96-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7ea96-116">A visszahívás ellenőrzésének lépései a következő [cikkben](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)olvashatók.</span><span class="sxs-lookup"><span data-stu-id="7ea96-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7ea96-117">E-mail-üzenetek keresése és törlése a szervezetben</span><span class="sxs-lookup"><span data-stu-id="7ea96-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7ea96-118">Ha nem globális rendszergazda, a fiókját fel kell vennie az eDiscovery-kezelő szerepkörbe vagy a megfelelőségi keresési felügyeleti szerepkörbe az üzenetek kereséséhez.</span><span class="sxs-lookup"><span data-stu-id="7ea96-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7ea96-119">Üzenetek törléséhez csatlakoznia kell a szervezeti vagy a keresési és törlési felügyeleti szerepkörhöz.</span><span class="sxs-lookup"><span data-stu-id="7ea96-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7ea96-120">Ezek a szerepkörök engedélyei a [biztonsági és megfelelőségi központban](https://go.microsoft.com/fwlink/?linkid=2083731)lesznek kiosztva.</span><span class="sxs-lookup"><span data-stu-id="7ea96-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7ea96-121">A törlendő üzenet megtalálásához [hozzon létre egy keresési tartalmat](https://docs.microsoft.com/microsoft-365/compliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="7ea96-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7ea96-122">[Csatlakozás a biztonsági és megfelelőségi központ powershellhez](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="7ea96-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7ea96-123">Többtényezős hitelesítés esetén a [Csatlakozás a Microsoft 365 biztonsági és megfelelőségi központ powershellhez többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)című témakörben tájékozódhat.</span><span class="sxs-lookup"><span data-stu-id="7ea96-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>