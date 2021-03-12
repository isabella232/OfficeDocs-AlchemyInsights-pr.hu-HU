---
title: Hozzáférés megtagadva üzenetek hibaelhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707956"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="52b84-102">Hozzáférés megtagadva üzenetek hibaelhárítása a SharePointban és a OneDrive Felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="52b84-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="52b84-103">Ha egy Hozzáférés megtagadva üzenet jelenik meg, amikor egy SharePoint/OneDrive Felügyeleti központot próbál meg böngészni, győződjön meg arról, hogy hozzárendelt egy licencet [a felhasználóhoz.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="52b84-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="52b84-104">Ha a felhasználó rendelkezik licenccel, akkor azt is meg kell győződni arról, hogy olyan rendszergazdai szerepkört kap, amely hozzáférhet [a](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) felügyeleti központokhoz.</span><span class="sxs-lookup"><span data-stu-id="52b84-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="52b84-105">Ez a probléma akkor is előfordulhat, ha egy felhasználót törölnek, majd újra létrehoznak ugyanazokkal az egyszerű felhasználónévvel.</span><span class="sxs-lookup"><span data-stu-id="52b84-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="52b84-106">Az új fiók egy másik PUID (Passport Unique ID) értékkel jön létre.</span><span class="sxs-lookup"><span data-stu-id="52b84-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="52b84-107">Amikor a felhasználó megpróbál hozzáférni egy webhelycsoporthoz vagy a OneDrive-jukhoz, helytelen PUID azonosítót adott meg.</span><span class="sxs-lookup"><span data-stu-id="52b84-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="52b84-108">A második forgatókönyv az Active Directory szervezeti egységekkel való címtár-szinkronizálást foglalja magában.</span><span class="sxs-lookup"><span data-stu-id="52b84-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="52b84-109">Ha a felhasználók már bejelentkeztek a SharePointba, majd áthelyezik őket egy másik szervezeti webhelyre, és újraszinkron módon szinkronizálják őket a SharePointtal, akkor előfordulhat, hogy ez a probléma jelentkezik.</span><span class="sxs-lookup"><span data-stu-id="52b84-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="52b84-110">A probléma megoldásához állítsa vissza az eredeti egyszerű felhasználószámot a Felhasználó visszaállítása [a Microsoft 365-ben](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)a cikkben található lépésekkel.</span><span class="sxs-lookup"><span data-stu-id="52b84-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="52b84-111">Megjegyzés: Ha a OneDrive vagy a SharePoint Felügyeleti központ nem érhető el több, korábban hozzáféréssel rendelkező felhasználónak, átmeneti szolgáltatásbeli probléma lehet.</span><span class="sxs-lookup"><span data-stu-id="52b84-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="52b84-112">[Ellenőrizze a szolgáltatás állapot-irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="52b84-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


