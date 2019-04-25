---
title: Postafiók első 126 nem található hibaüzenet az OWA?
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 126
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: fe8119c300e99170da4f338f2420b1229ab24bea
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32400827"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="96112-102">Az első hiba nem található a weben Outlook postafiók?</span><span class="sxs-lookup"><span data-stu-id="96112-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="96112-103">Ha a **postaláda nem található a következő** hibaüzenet jelenik meg az Outlook programot a weben, az Outlook a weben való kapcsolódáshoz használt fiók nem rendelkezik az Exchange Online licencet, és ezért nincs postaláda a fiókjához társított.</span><span class="sxs-lookup"><span data-stu-id="96112-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="96112-104">A rendszergazda is licenc hozzárendelése a fiók az alábbiak szerint:</span><span class="sxs-lookup"><span data-stu-id="96112-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="96112-105">Nyissa meg a [Microsoft 365 felügyeleti központ](https://portal.office.com/adminportal/home#/homepage) , és **aktív felhasználók**csoportban jelölje be a **felhasználó szerkesztése**.</span><span class="sxs-lookup"><span data-stu-id="96112-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="96112-106">Megnyitó **felhasználó szerkesztése** lapon jelölje ki a felhasználót.</span><span class="sxs-lookup"><span data-stu-id="96112-106">In the **Edit a user** page that opens, select the user.</span></span> <span data-ttu-id="96112-107">A megnyitó felhasználó tulajdonságlapon kattintson **terméklicencek**a **Szerkesztés** gombra.</span><span class="sxs-lookup"><span data-stu-id="96112-107">In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="96112-108">**Terméklicencek** lapon válassza ki a megfelelő **helyre** értéket, és rendel hozzá, amely tartalmazza az Exchange Online licencet (a licenc részletes adatainak megtekintéséhez bontsa ki).</span><span class="sxs-lookup"><span data-stu-id="96112-108">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="96112-109">Ha elkészült, kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="96112-109">When you're finished, click **Save**.</span></span>
