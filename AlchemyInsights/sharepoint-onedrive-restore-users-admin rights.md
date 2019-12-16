---
title: Az OneDrive for Business webhelyeknek való hozzáférés megtagadási problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051607"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="2e584-102">Az OneDrive for Business webhelyeknek való hozzáférés megtagadási problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="2e584-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="2e584-103">Ez a probléma leggyakrabban akkor jelentkezik, ha egy felhasználó törlődik, és ugyanazzal az egyszerű felhasználónévvel (UPN) újra létrehozza.</span><span class="sxs-lookup"><span data-stu-id="2e584-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="2e584-104">Az új fiók a Passport egyedi AZONOSÍTÓI értékének használatával jön létre.</span><span class="sxs-lookup"><span data-stu-id="2e584-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="2e584-105">Mikor a felhasználó megpróbál-hoz belépés egy telek gyűjtemény vagy-uk OneDrive, a felhasználó birtokol egy rossz PUID.</span><span class="sxs-lookup"><span data-stu-id="2e584-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="2e584-106">A második forgatókönyv egy Active Directory szervezeti egységgel (OU) rendelkező címtár-szinkronizálást foglal magában.</span><span class="sxs-lookup"><span data-stu-id="2e584-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="2e584-107">Ha a felhasználók már bejelentkezett a SharePoint-ba, majd egy másik szervezeti egységbe kerülnek, és újra átviszik a SharePoint-alkalmazással, akkor a problémát tapasztalhatják.</span><span class="sxs-lookup"><span data-stu-id="2e584-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="2e584-108">A probléma megoldásához állítsa vissza az eredeti UPN-t a cikk lépéseinek segítségével, a [felhasználó visszaállítása az Office 365-ben](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="2e584-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="2e584-109">Ha Ön nem tud visszaad a eredeti felhasználó Önnek kellene eltávolít a régi felhasználó-ból OneDrive telek használ ezek lép, [eltávolít egy felhasználó-ból felhasználó értesít oldalra dől]().</span><span class="sxs-lookup"><span data-stu-id="2e584-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="2e584-110">Után ez megtett, tudod igazol a felhasználó birtokol admin jogok-hoz OneDrive telek mellett alábbiak a lép-hoz [összead admins ' részére egy használók ' OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="2e584-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="2e584-111">A jogosultsági szintekkel kapcsolatos további tudnivalókért tanulmányozza a [SharePoint rendszerben a jogosultsági szintek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakört.</span><span class="sxs-lookup"><span data-stu-id="2e584-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
