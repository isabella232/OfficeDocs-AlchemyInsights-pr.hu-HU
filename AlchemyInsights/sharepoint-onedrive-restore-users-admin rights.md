---
title: Az Access által a OneDrive Vállalati verzió webhelyeire irányuló üzenetek hibáinak elhárítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692803"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="ad79c-102">Az Access által a OneDrive Vállalati verzió webhelyeire irányuló üzenetek hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="ad79c-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="ad79c-103">Ez a probléma leggyakrabban akkor fordul elő, ha egy felhasználót törölnek, és újra létrehoznak ugyanazzal az egyszerű felhasználónévvel (UPN).</span><span class="sxs-lookup"><span data-stu-id="ad79c-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ad79c-104">Az új fiók egy másik PUID (Passport Unique ID) érték kel jön létre.</span><span class="sxs-lookup"><span data-stu-id="ad79c-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ad79c-105">Amikor a felhasználó megpróbál hozzáférni egy webhelycsoporthoz vagy a OneDrive-hoz, a felhasználó nem megfelelő PUID azonosítóval rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="ad79c-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ad79c-106">A második forgatókönyv a címtár-szinkronizálás az Active Directory szervezeti egységgel (OU).</span><span class="sxs-lookup"><span data-stu-id="ad79c-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ad79c-107">Ha a felhasználók már bejelentkeztek a SharePointba, majd áthelyezték őket egy másik szervezeti egységbe, és újraszinkronizálták őket a SharePointtal, akkor ezt a problémát tapasztalhatják.</span><span class="sxs-lookup"><span data-stu-id="ad79c-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="ad79c-108">A probléma megoldásához állítsa vissza az eredeti felhasználói felületet a cikkben ismertetett lépésekkel, a Felhasználó visszaállítása a [Microsoft 365 alkalmazásban](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ad79c-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="ad79c-109">Ha nem tudja visszaállítani az eredeti felhasználót, távolítsa el a régi felhasználót a OneDrive-webhelyről az alábbi lépésekkel, [távolítsa el a felhasználót a felhasználói adatok listájából]().</span><span class="sxs-lookup"><span data-stu-id="ad79c-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="ad79c-110">Miután ez megtörtént, ellenőrizheti, hogy a felhasználó rendszergazdai jogokkal rendelkezik-e a OneDrive-webhelyen, ha a [Rendszergazda hozzáadása a felhasználó OneDrive-jához](https://docs.microsoft.com/sharepoint/manage-user-profiles) című lépéseit követve ellenőrzi.</span><span class="sxs-lookup"><span data-stu-id="ad79c-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="ad79c-111">A jogosultsági szintekről a [SharePoint engedélyszintjeinek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című cikkben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="ad79c-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
