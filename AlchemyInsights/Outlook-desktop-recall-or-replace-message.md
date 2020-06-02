---
title: E-mail visszahívása vagy cseréje az Outlook Asztalon
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502321"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="ca746-102">Outlook-e-mail üzenet visszahívása vagy cseréje</span><span class="sxs-lookup"><span data-stu-id="ca746-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="ca746-103">Rendszergazdaként **visszahívhatja az üzeneteket a PowerShellt használó felhasználók nevében.**</span><span class="sxs-lookup"><span data-stu-id="ca746-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ca746-104">A felügyeleti központból nem lehet üzeneteket visszahívni.</span><span class="sxs-lookup"><span data-stu-id="ca746-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ca746-105">Csak a **szervezeten belüli személyeknek küldött üzeneteket tudja visszahívni.**</span><span class="sxs-lookup"><span data-stu-id="ca746-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ca746-106">Ha például egy Gmail-címre küldték az üzenetet, nem tudja visszahívni.</span><span class="sxs-lookup"><span data-stu-id="ca746-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ca746-107">Az **Outlook 2016-ból küldött üzeneteket csak pc-n lehet visszahívni.**</span><span class="sxs-lookup"><span data-stu-id="ca746-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ca746-108">Ha egy felhasználó üzenetet küld a Mac Outlookkal vagy a Webes Outlookkal, nem tudja visszahívni.</span><span class="sxs-lookup"><span data-stu-id="ca746-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ca746-109">E-mail üzenet visszahívása vagy cseréje:</span><span class="sxs-lookup"><span data-stu-id="ca746-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ca746-110">Az Outlook ablakbal bal oldalán lévő mappaablakban jelölje ki az Elküldött elemek mappát.</span><span class="sxs-lookup"><span data-stu-id="ca746-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ca746-111">A megnyitáshoz kattintson duplán a visszahívni kívánt üzenetre.</span><span class="sxs-lookup"><span data-stu-id="ca746-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ca746-112">Kattintson az **Üzenet** fülre, majd az Üzenet **visszahívása művelet**  >  **parancsra.**</span><span class="sxs-lookup"><span data-stu-id="ca746-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ca746-113">Jelölje be **az Üzenet olvasatlan példányainak törlése** vagy Az **olvasatlan másolatok törlése és lecserélése új üzenetre**jelölőnégyzetet, majd kattintson **az OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="ca746-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ca746-114">Ha helyettesítő üzenetet küld, írja meg az üzenetet, majd válassza a **Küldés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ca746-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ca746-115">Az üzenet-visszahívás sikeres vagy sikertelen volt, a címzett Outlook ban megadott beállításaitól függ.</span><span class="sxs-lookup"><span data-stu-id="ca746-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ca746-116">A visszahívás ellenőrzéséhez ezt a [cikket](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)lásd.</span><span class="sxs-lookup"><span data-stu-id="ca746-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ca746-117">E-mailek keresése és törlése a szervezetben</span><span class="sxs-lookup"><span data-stu-id="ca746-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ca746-118">Ha ön nem globális rendszergazda, az üzenetek kereséséhez hozzá kell adni a fiókját az elektronikus adatfeltárás-kezelői szerepkörhöz vagy a Megfelelőségi keresés felügyeleti szerepköréhez.</span><span class="sxs-lookup"><span data-stu-id="ca746-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ca746-119">Az üzenetek törléséhez csatlakoznia kell a Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és törlés felügyeleti szerepkörhöz.</span><span class="sxs-lookup"><span data-stu-id="ca746-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ca746-120">A szerepkörökhöz tartozó engedélyek a [Biztonsági és megfelelőségi központban](https://go.microsoft.com/fwlink/?linkid=2083731)vannak hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="ca746-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ca746-121">[Hozzon létre egy tartalomkeresést](https://docs.microsoft.com/microsoft-365/compliance/content-search) a törlandó üzenet megkereséséhez.</span><span class="sxs-lookup"><span data-stu-id="ca746-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ca746-122">[Csatlakozzon a Security and Compliance Center PowerShell hez.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="ca746-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ca746-123">Ha többtényezős hitelesítést használ, olvassa el [a Csatlakozás a Microsoft 365 biztonsági és megfelelőségi központPowerShell hez többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)című témakört.</span><span class="sxs-lookup"><span data-stu-id="ca746-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>