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
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767664"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="dc666-102">Hozzáférés megtagadva üzenetek hibaelhárítása a SharePoint/OneDrive felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="dc666-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="dc666-103">Ha egy SharePoint-vagy OneDrive felügyeleti központra való tallózáskor hozzáférés-megtagadási üzenetet kap, győződjön meg arról, hogy a [felhasználónak licencet kell rendelnie a felhasználóhoz](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="dc666-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="dc666-104">Ha a felhasználó rendelkezik licenccel, gondoskodnia kell arról is, hogy a rendszergazdai központokhoz hozzáférő [rendszergazdai szerepkört rendeljen](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="dc666-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="dc666-105">Ez a probléma akkor is előfordulhat, ha egy felhasználó törlődik, és újból létrejön ugyanazzal a egyszerű felhasználónévsel (UPN).</span><span class="sxs-lookup"><span data-stu-id="dc666-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="dc666-106">Az új fiókot egy másik PUID (Passport egyedi azonosító) használatával hozza létre.</span><span class="sxs-lookup"><span data-stu-id="dc666-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="dc666-107">Amikor a felhasználó megkísérel hozzáférni egy webhelycsoportban vagy a OneDrive, a felhasználó helytelen PUID rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="dc666-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="dc666-108">A második forgatókönyv a címtár-szinkronizálást jelenti Active Directory-beli szervezeti egységgel (OU).</span><span class="sxs-lookup"><span data-stu-id="dc666-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="dc666-109">Ha a felhasználók már bejelentkezett a SharePointba, és egy másik szervezeti egységbe vannak áthelyezve, és a SharePointtal újra szinkronizálják őket, előfordulhat, hogy ez a probléma tapasztalható.</span><span class="sxs-lookup"><span data-stu-id="dc666-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="dc666-110">A probléma megoldásához vissza kell állítania az eredeti UPN-t a cikkben ismertetett lépésekkel, ha [vissza szeretne állítani egy felhasználót a Microsoft 365-ban](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="dc666-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="dc666-111">Megjegyzés: Ha egy OneDrive vagy SharePoint felügyeleti központ nem érhető el több olyan felhasználónál, aki korábban hozzáféréssel rendelkezik, előfordulhat, hogy ideiglenes szolgáltatási probléma van.</span><span class="sxs-lookup"><span data-stu-id="dc666-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="dc666-112">[Ellenőrizze a szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="dc666-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


