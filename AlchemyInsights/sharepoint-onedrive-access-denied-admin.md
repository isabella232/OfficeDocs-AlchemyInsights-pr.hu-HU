---
title: Hozzáférés-megtagadási üzenetek – problémamegoldás
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051427"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="755eb-102">A SharePoint/OneDrive Admin Center rendszerben található hozzáférés-megtagadási üzenetek – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="755eb-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="755eb-103">Ha a SharePoint/OneDrive Admin Center webhely megnyitásakor hozzáférés-megtagadási üzenetet kap, akkor ellenőrizze, hogy [a felhasználóhoz rendel](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)-e licencet.</span><span class="sxs-lookup"><span data-stu-id="755eb-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="755eb-104">Ha a felhasználó rendelkezik licenccel, győződjön meg arról is, hogy hozzá vannak-e [rendelve rendszergazdai szerepkör](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , amely hozzáfér az adminisztrációs központokhoz.</span><span class="sxs-lookup"><span data-stu-id="755eb-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="755eb-105">Ez a probléma akkor is előfordulhat, ha egy felhasználót töröl, és ugyanazzal az egyszerű felhasználónévvel (UPN) újra létrehozza.</span><span class="sxs-lookup"><span data-stu-id="755eb-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="755eb-106">Az új fiók a Passport egyedi AZONOSÍTÓI értékének használatával jön létre.</span><span class="sxs-lookup"><span data-stu-id="755eb-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="755eb-107">Mikor a felhasználó megpróbál-hoz belépés egy telek gyűjtemény vagy-uk OneDrive, a felhasználó birtokol egy rossz PUID.</span><span class="sxs-lookup"><span data-stu-id="755eb-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="755eb-108">A második forgatókönyv egy Active Directory szervezeti egységgel (OU) rendelkező címtár-szinkronizálást foglal magában.</span><span class="sxs-lookup"><span data-stu-id="755eb-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="755eb-109">Ha a felhasználók már bejelentkezett a SharePoint-ba, majd egy másik szervezeti egységbe kerülnek, és újra átviszik a SharePoint-alkalmazással, akkor a problémát tapasztalhatják.</span><span class="sxs-lookup"><span data-stu-id="755eb-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="755eb-110">A probléma megoldásához állítsa vissza az eredeti UPN-t a cikkben leírt lépésekkel, [állítsa vissza a felhasználót az Office 365-ben](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="755eb-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="755eb-111">Jegyzék Ha egy OneDrive vagy SharePoint admin központ van nem elérhető-hoz sokszoros használók ki korábban belépés, ott május lenni egy ideiglenes szolgáltatás kérdés.</span><span class="sxs-lookup"><span data-stu-id="755eb-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="755eb-112">[Ellenőrizze a szolgáltatás állapotirányítópultját](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="755eb-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


