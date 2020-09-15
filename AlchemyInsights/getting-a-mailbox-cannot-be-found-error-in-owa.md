---
title: az OWA alkalmazásban nem található az 126-ös postaláda-hiba
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706752"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="bfde7-102">Nem található a postaláda hibája a webes Outlookban?</span><span class="sxs-lookup"><span data-stu-id="bfde7-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="bfde7-103">Ha a webes Outlookot használja, és a **postaládáját nem sikerült megtalálni** , akkor a webes Outlookhoz való csatlakozáshoz használt fiók nem rendelkezik Exchange Online-licenccel, ezért a fiókhoz nincs társítva postaláda.</span><span class="sxs-lookup"><span data-stu-id="bfde7-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="bfde7-104">A rendszergazda az alábbi lépésekkel rendelhet licencet a fiókjához:</span><span class="sxs-lookup"><span data-stu-id="bfde7-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="bfde7-105">Nyissa meg a [Microsoft 365 felügyeleti központját](https://portal.office.com/adminportal/home#/homepage) , és nyissa meg az **aktív felhasználók** szakaszt a **felhasználók** csoportban, és jelölje ki azt a felhasználót, aki látta a hibát.</span><span class="sxs-lookup"><span data-stu-id="bfde7-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="bfde7-106">A megnyíló felhasználói lapon nyissa meg a **licencek és alkalmazások** szakaszt, válassza ki a megfelelő **tartózkodási helyet** , és rendelje hozzá az Exchange Online-t tartalmazó licencet (bontsa ki a licencet a részletek megjelenítéséhez).</span><span class="sxs-lookup"><span data-stu-id="bfde7-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="bfde7-107">Ha végzett, kattintson a **módosítások mentése**gombra.</span><span class="sxs-lookup"><span data-stu-id="bfde7-107">When you're finished, click **Save changes**.</span></span>
