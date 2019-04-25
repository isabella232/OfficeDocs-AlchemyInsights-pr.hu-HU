---
title: Az Outlook asztali visszahívás vagy e-mail üzenet csere
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389704"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="655c2-102">Visszahívni vagy kicserélni egy e-mailt</span><span class="sxs-lookup"><span data-stu-id="655c2-102">Recall or replace an email message</span></span>

- <span data-ttu-id="655c2-103">Mint a rendszergazda **Visszahívási üzenet PowerShell segítségével a felhasználók nevében**is.</span><span class="sxs-lookup"><span data-stu-id="655c2-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="655c2-104">Az admin center üzenetek nem tudja visszahívni.</span><span class="sxs-lookup"><span data-stu-id="655c2-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="655c2-105">**Csak a szervezet tagjai által küldött visszahívása üzeneteket**is.</span><span class="sxs-lookup"><span data-stu-id="655c2-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="655c2-106">Ha az üzenet a Gmail címre lett küldve, például nem emlékszünk rá.</span><span class="sxs-lookup"><span data-stu-id="655c2-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="655c2-107">Lehetőség van **csak a a PC-n Outlook 2016 küldött üzenetek visszahívása**.</span><span class="sxs-lookup"><span data-stu-id="655c2-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="655c2-108">A felhasználó Outlook for Mac és a weben az Outlook üzenetet küld, ha nem tudja visszahívni.</span><span class="sxs-lookup"><span data-stu-id="655c2-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="655c2-109">A visszahívással vagy cserélje ki egy e-mail üzenetet:</span><span class="sxs-lookup"><span data-stu-id="655c2-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="655c2-110">A mappalistán az Outlook ablak a bal oldalon jelölje be az elküldött elemek mappába.</span><span class="sxs-lookup"><span data-stu-id="655c2-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="655c2-111">Kattintson duplán a nyissa meg a visszahívni kívánt üzenetet.</span><span class="sxs-lookup"><span data-stu-id="655c2-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="655c2-112">Kattintson az **üzenet** fülre, és válassza a **Műveletek** > **Az üzenet visszahívása**.</span><span class="sxs-lookup"><span data-stu-id="655c2-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="655c2-113">**Törli az üzenet olvasatlan példányait** , vagy **törli olvasatlan példányait és cserélje le egy új üzenetet**, és kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="655c2-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="655c2-114">Ha csere üzenetet küldünk, írjuk meg az üzenetet, és válassza a **Küldés**.</span><span class="sxs-lookup"><span data-stu-id="655c2-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="655c2-115">A sikeres vagy sikertelen üzenet-visszahívásról függ, hogy a címzett az Outlook beállításait.</span><span class="sxs-lookup"><span data-stu-id="655c2-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="655c2-116">A visszahívás ellenőrzése, olvassa el [a](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)lépéseket.</span><span class="sxs-lookup"><span data-stu-id="655c2-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="655c2-117">Keresse meg, és a szervezet e-mail üzenetek törlése</span><span class="sxs-lookup"><span data-stu-id="655c2-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="655c2-118">Ha Ön nem egy globális felügyeleti, a fiók az elektronikus adatok feltárása kezelője szerepkör vagy üzenetek kereséséhez való keresés szerepkör hozzá kell adni.</span><span class="sxs-lookup"><span data-stu-id="655c2-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="655c2-119">Üzenetek törlése, szüksége lesz a Szervezetkezelés szerepkör vagy a Keresés és a kiürítés szerepkör csatlakozni.</span><span class="sxs-lookup"><span data-stu-id="655c2-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="655c2-120">Ezek a szerepkörök az engedélyeket a [biztonsági és kompatibilitási központ](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="655c2-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="655c2-121">[Keresés a tartalom létrehozása](https://docs.microsoft.com/office365/securitycompliance/content-search) az üzenet törlése.</span><span class="sxs-lookup"><span data-stu-id="655c2-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="655c2-122">[Biztonsági és Megfelelési központba PowerShell kapcsolódni](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="655c2-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="655c2-123">Többtényezős hitelesítést használ, lásd a [Csatlakozás az Office 365 biztonsági és kompatibilitási központ PowerShell többtényezős hitelesítést használ](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="655c2-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>