---
title: Teljesítménnyel kapcsolatos problémák – SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771246"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="c2d09-102">A SharePoint vagy a OneDrive lassú, elérhetetlen vagy nem elérhető több felhasználó esetében</span><span class="sxs-lookup"><span data-stu-id="c2d09-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="c2d09-103">Ha egy OneDrive vagy SharePoint-webhely nem érhető el több olyan felhasználónál, aki korábban hozzáféréssel rendelkezik, előfordulhat, hogy ideiglenes szolgáltatási probléma van.</span><span class="sxs-lookup"><span data-stu-id="c2d09-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="c2d09-104">[Ellenőrizze a szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c2d09-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="c2d09-105">**A felhasználó hozzáadása és licence**</span><span class="sxs-lookup"><span data-stu-id="c2d09-105">**Add and license the user**</span></span>

<span data-ttu-id="c2d09-106">Győződjön meg arról, hogy [licenceket rendel a felhasználókhoz a Microsoft 365 vállalati](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)verziójában.</span><span class="sxs-lookup"><span data-stu-id="c2d09-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="c2d09-107">**Engedélyek hozzárendelése**</span><span class="sxs-lookup"><span data-stu-id="c2d09-107">**Assign Permissions**</span></span>

<span data-ttu-id="c2d09-108">Ha a felhasználó SharePoint-licenccel rendelkezik, és továbbra is egy hozzáférés-megtagadási üzenetet kap, győződjön meg arról, hogy rendelkeznek a [megfelelő jogosultsági szinttel](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="c2d09-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="c2d09-109">**A hozzáférés kérése funkció használata**</span><span class="sxs-lookup"><span data-stu-id="c2d09-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="c2d09-110">A [hozzáférési kérés funkció](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) lehetővé teszi, hogy a felhasználók hozzáférést kérjen olyan tartalmakhoz, amelyekre jelenleg nincs engedélye.</span><span class="sxs-lookup"><span data-stu-id="c2d09-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="c2d09-111">**Hozzáférés megtagadását okozó egyéni parancsfájlok engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="c2d09-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="c2d09-112">Bizonyos esetekben az *egyéni parancsfájl engedélyezése* funkció a hozzáférés megtagadását okozhatja.</span><span class="sxs-lookup"><span data-stu-id="c2d09-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="c2d09-113">Az érintett szolgáltatások listáját, a biztonsági megfontolásokat és a funkció letiltását is lehetővé teszi.</span><span class="sxs-lookup"><span data-stu-id="c2d09-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="c2d09-114">Kérjük, keresse meg az [egyéni parancsfájlok engedélyezése vagy letiltása című leírást](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="c2d09-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

