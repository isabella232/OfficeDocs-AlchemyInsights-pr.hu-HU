---
title: Az Outlook asztali visszahívása vagy lecserélése az e-mail üzenetre
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496113"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="482df-102">Outlook e-mail üzenet visszahívása vagy lecserélése</span><span class="sxs-lookup"><span data-stu-id="482df-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="482df-103">Mint az admin, akkor **felidézni üzeneteket nevében a felhasználók segítségével PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="482df-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="482df-104">Nem lehet visszahívni az üzeneteket az Admin Center.</span><span class="sxs-lookup"><span data-stu-id="482df-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="482df-105">Csak a **szervezetben lévő személyeknek elküldött üzeneteket lehet visszahívni**.</span><span class="sxs-lookup"><span data-stu-id="482df-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="482df-106">Ha például az üzenetet Gmail-címre küldték, nem lehet visszahívni.</span><span class="sxs-lookup"><span data-stu-id="482df-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="482df-107">**Csak az Outlook 2016-ből küldött üzenetek visszahívhatók a számítógépen**.</span><span class="sxs-lookup"><span data-stu-id="482df-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="482df-108">Ha a felhasználó az Outlook for Mac vagy az Outlook alkalmazással küld üzenetet a weben, akkor nem tudja felidézni.</span><span class="sxs-lookup"><span data-stu-id="482df-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="482df-109">E-mail üzenet felidézése vagy cseréje:</span><span class="sxs-lookup"><span data-stu-id="482df-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="482df-110">Az Outlook ablakának bal oldalán található mappalistán jelölje ki az elküldött elemek mappát.</span><span class="sxs-lookup"><span data-stu-id="482df-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="482df-111">Kattintson duplán a visszahívni kívánt üzenetre.</span><span class="sxs-lookup"><span data-stu-id="482df-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="482df-112">Válassza az **üzenet** fület, majd válassza a **műveletek** > **visszahívása ezt az üzenetet**.</span><span class="sxs-lookup"><span data-stu-id="482df-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="482df-113">Jelölje be az **üzenet olvasatlan másolatainak törlése** vagy az **olvasatlan másolatok törlése és a lecserélés egy új üzenetre**választógombot, majd kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="482df-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="482df-114">Ha cserecikk üzenetet küldünk, írjuk be az üzenetet, majd nyomjuk meg a **küld**választógombot.</span><span class="sxs-lookup"><span data-stu-id="482df-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="482df-115">Az üzenet-visszahívás sikere vagy sikertelenje a címzettek Outlook programban megadott beállításaitól függ.</span><span class="sxs-lookup"><span data-stu-id="482df-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="482df-116">A visszahívás ellenőrzéséhez szükséges lépések a [jelen cikkben](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)találhatók.</span><span class="sxs-lookup"><span data-stu-id="482df-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="482df-117">E-mail üzenetek keresése és törlése a szervezeten belül</span><span class="sxs-lookup"><span data-stu-id="482df-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="482df-118">Ha Ön nem egy globális rendszergazda, akkor fiókját hozzá kell adni az eDiscovery Manager szerepkörhöz vagy a megfelelőségi keresés felügyeleti szerepkörhöz az üzenetek kereséséhez.</span><span class="sxs-lookup"><span data-stu-id="482df-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="482df-119">Az üzenetek törléséhez csatlakoznunk kell a Szervezetkezelés szerepkörcsoporthoz vagy a keresés és tisztítás felügyeleti szerepkörhöz.</span><span class="sxs-lookup"><span data-stu-id="482df-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="482df-120">Az ezekhez a szerepkörökhöz tartozó engedélyeket a [biztonsági és megfelelőségi központ](https://go.microsoft.com/fwlink/?linkid=2083731)rendeli hozzá.</span><span class="sxs-lookup"><span data-stu-id="482df-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="482df-121">[Hozzon létre egy tartalomkeresést](https://docs.microsoft.com/office365/securitycompliance/content-search) a törlendő üzenet megkereséséhez.</span><span class="sxs-lookup"><span data-stu-id="482df-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="482df-122">[Összeköt-hoz biztonság és engedékenység központ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="482df-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="482df-123">Többtényezős hitelesítés használata esetén tekintse meg [a Kapcsolódás az Office 365 biztonsági és megfelelőségi központ PowerShell környezethez a többtényezős hitelesítés használatával](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)című témakört.</span><span class="sxs-lookup"><span data-stu-id="482df-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>