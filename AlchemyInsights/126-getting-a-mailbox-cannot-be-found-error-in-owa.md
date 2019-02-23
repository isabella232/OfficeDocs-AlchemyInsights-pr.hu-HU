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
ms.custom: Adm_O365
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: b7d54e9fb29bf94ec540e6059e932ec33f326495
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/22/2019
ms.locfileid: "30209811"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="35b18-102">Az első hiba nem található a weben Outlook postafiók?</span><span class="sxs-lookup"><span data-stu-id="35b18-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="35b18-p101">Ha a **postaláda nem található a következő** hibaüzenet jelenik meg az Outlook programot a weben, az Outlook a weben való kapcsolódáshoz használt fiók nem rendelkezik az Exchange Online licencet, és ezért nincs postaláda a fiókjához társított. A rendszergazda is licenc hozzárendelése a fiók az alábbiak szerint:</span><span class="sxs-lookup"><span data-stu-id="35b18-p101">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account. Your admin can assign a license to your account by following these steps:</span></span> 
  
1. <span data-ttu-id="35b18-105">Nyissa meg a [Microsoft 365 felügyeleti központ](https://portal.office.com/adminportal/home#/homepage) , és **aktív felhasználók**csoportban jelölje be a **felhasználó szerkesztése**.</span><span class="sxs-lookup"><span data-stu-id="35b18-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>
    
2. <span data-ttu-id="35b18-p102">Megnyitó **felhasználó szerkesztése** lapon jelölje ki a felhasználót. A megnyitó felhasználó tulajdonságlapon kattintson **terméklicencek**a **Szerkesztés** gombra.</span><span class="sxs-lookup"><span data-stu-id="35b18-p102">In the **Edit a user** page that opens, select the user. In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>
    
3. <span data-ttu-id="35b18-p103">**Terméklicencek** lapon válassza ki a megfelelő **helyre** értéket, és rendel hozzá, amely tartalmazza az Exchange Online licencet (a licenc részletes adatainak megtekintéséhez bontsa ki). Ha elkészült, kattintson a **Mentés**gombra.</span><span class="sxs-lookup"><span data-stu-id="35b18-p103">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details). When you're finished, click **Save**.</span></span>
    

