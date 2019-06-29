---
title: Hibaelhárítás a hozzáférés megtagadva a OneDrive üzenetek üzleti helyek
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354799"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="42548-102">Hibaelhárítás a hozzáférés megtagadva a OneDrive üzenetek üzleti helyek</span><span class="sxs-lookup"><span data-stu-id="42548-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="42548-103">Ez a probléma leggyakrabban akkor fordul elő, amikor a felhasználó törli, és újra létrehozza a ugyanolyan egyszerű felhasználónév (UPN).</span><span class="sxs-lookup"><span data-stu-id="42548-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="42548-104">Az új fiók jön létre egy másik értéket PUID (Passport egyedi azonosító) segítségével.</span><span class="sxs-lookup"><span data-stu-id="42548-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="42548-105">Ha a felhasználó megpróbál hozzáférni egy webhelycsoport vagy a OneDrive, a felhasználó rendelkezik egy helytelen PUID.</span><span class="sxs-lookup"><span data-stu-id="42548-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="42548-106">A második forgatókönyv magában foglalja a könyvtár szinkronizálás az Active Directory szervezeti egységet (OU).</span><span class="sxs-lookup"><span data-stu-id="42548-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="42548-107">Ha a felhasználó rendelkezik már bejelentkezett a SharePoint, majd átkerül egy másik szervezeti egység és SharePoint resynced, akkor ez a probléma tapasztalhatnak.</span><span class="sxs-lookup"><span data-stu-id="42548-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="42548-108">A probléma megoldásához a cikk[az Office 365 rendszerben a felhasználó visszaállítási](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)lépéseket az eredeti UPN kell visszaállítani.</span><span class="sxs-lookup"><span data-stu-id="42548-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="42548-109">Miután ez elkészült, a felhasználó rendelkezik rendszergazdai jogokat a OneDrive webhelyen történő [hozzáadása admin által a felhasználó OneDrive a](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) lépéseket követve ellenőrizheti</span><span class="sxs-lookup"><span data-stu-id="42548-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="42548-110">Jogosultsági szintekkel kapcsolatos további tudnivalókért lásd a cikk [SharePoint jogosultsági szintek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="42548-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
