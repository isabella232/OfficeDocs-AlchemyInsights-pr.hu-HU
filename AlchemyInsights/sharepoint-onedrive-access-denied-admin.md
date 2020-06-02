---
title: Hozzáférés megtagadott üzenetek hibáinak elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505381"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="c5e80-102">Hozzáférés megtagadott üzenetek hibái a Sharepoint/OneDrive Felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="c5e80-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="c5e80-103">Ha a Sharepoint/OneDrive Felügyeleti központ megtallásához megkísérelt hozzáférési üzenetet kap, győződjön meg arról, hogy [licencet rendelt a felhasználóhoz.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="c5e80-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="c5e80-104">Ha a felhasználó rendelkezik licenccel, győződjön meg arról is, hogy [rendszergazdai szerepkört kapnak,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) amely hozzáférhet a felügyeleti központokhoz.</span><span class="sxs-lookup"><span data-stu-id="c5e80-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="c5e80-105">Ez a probléma akkor is előfordulhat, ha egy felhasználót törölnek, és újra létrehoznak ugyanazzal a egyszerű felhasználónévvel (UPN).</span><span class="sxs-lookup"><span data-stu-id="c5e80-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c5e80-106">Az új fiók egy másik PUID (Passport Unique ID) érték kel jön létre.</span><span class="sxs-lookup"><span data-stu-id="c5e80-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c5e80-107">Amikor a felhasználó megpróbál hozzáférni egy webhelycsoporthoz vagy a OneDrive-hoz, a felhasználó nem megfelelő PUID azonosítóval rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="c5e80-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c5e80-108">A második forgatókönyv a címtár-szinkronizálás az Active Directory szervezeti egységgel (OU).</span><span class="sxs-lookup"><span data-stu-id="c5e80-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c5e80-109">Ha a felhasználók már bejelentkeztek a SharePointba, majd áthelyezték őket egy másik szervezeti egységbe, és újraszinkronizálták őket a SharePointtal, akkor ezt a problémát tapasztalhatják.</span><span class="sxs-lookup"><span data-stu-id="c5e80-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="c5e80-110">A probléma megoldásához állítsa vissza az eredeti felhasználói felületet a [Microsoft 365 felhasználójának visszaállítása](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)című cikkben ismertetett lépésekkel.</span><span class="sxs-lookup"><span data-stu-id="c5e80-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="c5e80-111">Megjegyzés: Ha egy OneDrive vagy SharePoint Felügyeleti központ nem érhető el több olyan felhasználó számára, akinek korábban hozzáférése volt, előfordulhat, hogy ideiglenes szolgáltatásprobléma lépett fel.</span><span class="sxs-lookup"><span data-stu-id="c5e80-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="c5e80-112">[Ellenőrizze a szolgáltatás állapotának irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="c5e80-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


