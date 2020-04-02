---
title: 126 A postaláda beszerzése nem található hiba az OWA-ban?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: e061ad6b74b27e3f0d597586cb2c8e31b8fa5d23
ms.sourcegitcommit: 83c644c35c2700dc515f091c8f41f9c283b89967
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43105241"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="9d017-102">Nem talál hibát a Webes Outlookban?</span><span class="sxs-lookup"><span data-stu-id="9d017-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="9d017-103">Ha a Webes Outlookot használja, és a **postaláda nem található** hiba miatt, akkor a webes Outlookhoz való csatlakozáshoz használt fiók nem rendelkezik Exchange Online-licenccel, ezért nincs postaládája a fiókhoz társítva.</span><span class="sxs-lookup"><span data-stu-id="9d017-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="9d017-104">A rendszergazda az alábbi lépésekkel rendelhet licencet a fiókjához:</span><span class="sxs-lookup"><span data-stu-id="9d017-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="9d017-105">Nyissa meg a [Microsoft 365 Felügyeleti központot,](https://portal.office.com/adminportal/home#/homepage) és a **Felhasználók** szakaszban nyissa meg az **Aktív felhasználók lehetőséget,** és válassza ki a hibát észlelő felhasználót.</span><span class="sxs-lookup"><span data-stu-id="9d017-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="9d017-106">A megnyíló felhasználói lapon nyissa meg a **Licencek és alkalmazások szakaszt,** válassza ki a megfelelő **helyértéket,** és rendeljen hozzá egy Exchange Online-t tartalmazó licencet (bontsa ki a licencet a részletek megtekintéséhez).</span><span class="sxs-lookup"><span data-stu-id="9d017-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="9d017-107">Ha végzett, kattintson **a Módosítások mentése**gombra.</span><span class="sxs-lookup"><span data-stu-id="9d017-107">When you're finished, click **Save changes**.</span></span>
