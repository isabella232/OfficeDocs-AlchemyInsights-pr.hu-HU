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
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691685"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="a9720-102">Hozzáférés megtagadva üzenetek hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="a9720-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="a9720-103">Ha a SharePoint Online-webhelyen való tallózáskor hozzáférés-megtagadásról tájékoztató üzenetet kap, kérjük, olvassa el az alábbi cikkeket.</span><span class="sxs-lookup"><span data-stu-id="a9720-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="a9720-104">**A felhasználó hozzáadása és licence**</span><span class="sxs-lookup"><span data-stu-id="a9720-104">**Add and License the user**</span></span>

<span data-ttu-id="a9720-105">Győződjön meg arról, hogy [licenceket rendel a felhasználókhoz a Microsoft 365 vállalati](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)verziójában.</span><span class="sxs-lookup"><span data-stu-id="a9720-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>

<span data-ttu-id="a9720-106">**Engedélyek hozzárendelése**</span><span class="sxs-lookup"><span data-stu-id="a9720-106">**Assign Permissions**</span></span>

<span data-ttu-id="a9720-107">Ha a felhasználó SharePoint-licenccel rendelkezik, és továbbra is egy hozzáférés-megtagadási üzenetet kap, győződjön meg arról, hogy rendelkeznek a [megfelelő jogosultsági szinttel](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a9720-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="a9720-108">**A hozzáférés kérése funkció használata**</span><span class="sxs-lookup"><span data-stu-id="a9720-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="a9720-109">A [hozzáférési kérés](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) funkció lehetővé teszi, hogy a felhasználók hozzáférést kérjen olyan tartalmakhoz, amelyekre jelenleg nincs engedélye.</span><span class="sxs-lookup"><span data-stu-id="a9720-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="a9720-110">**Hozzáférés megtagadását okozó egyéni parancsfájlok engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="a9720-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="a9720-111">Bizonyos esetekben az "egyéni parancsfájl engedélyezése" funkció a hozzáférés megtagadását is lehetővé teszi.</span><span class="sxs-lookup"><span data-stu-id="a9720-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="a9720-112">Az érintett szolgáltatások listáját, a biztonsági megfontolásokat és a funkció letiltását is lehetővé teszi.</span><span class="sxs-lookup"><span data-stu-id="a9720-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a9720-113">Kérjük, keresse meg, [engedélyezze vagy megelőzze az egyéni parancsfájlokat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="a9720-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="a9720-114">Megjegyzés: Ha egy OneDrive vagy SharePoint-webhely nem érhető el több olyan felhasználónál, aki korábban hozzáféréssel rendelkezik, előfordulhat, hogy ideiglenes szolgáltatási probléma van.</span><span class="sxs-lookup"><span data-stu-id="a9720-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a9720-115">[Ellenőrizze a szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a9720-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

