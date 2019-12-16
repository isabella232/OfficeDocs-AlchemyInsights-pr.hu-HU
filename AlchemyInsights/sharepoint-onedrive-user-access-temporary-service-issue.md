---
title: Teljesítménnyel kapcsolatos problémák-SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053803"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="c106f-102">SharePoint vagy OneDrive lassú, nem elérhető vagy nem érhető el több felhasználó számára</span><span class="sxs-lookup"><span data-stu-id="c106f-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="c106f-103">Ha egy OneDrive vagy SharePoint webhely nem érhető el több olyan felhasználó számára, akik korábban már hozzáfértek, akkor lehet, hogy ideiglenes szervizhiba történt.</span><span class="sxs-lookup"><span data-stu-id="c106f-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="c106f-104">[Ellenőrizze a szolgáltatás állapotirányítópultját](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c106f-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="c106f-105">**A felhasználó hozzáadása és licence**</span><span class="sxs-lookup"><span data-stu-id="c106f-105">**Add and license the user**</span></span>

<span data-ttu-id="c106f-106">Győződjön meg arról, hogy [licenceket rendel az Office 365 for Business felhasználókhoz](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="c106f-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="c106f-107">**Engedélyek hozzárendelése**</span><span class="sxs-lookup"><span data-stu-id="c106f-107">**Assign Permissions**</span></span>

<span data-ttu-id="c106f-108">Ha a felhasználóhoz SharePoint-licenc van rendelve, és továbbra is kap hozzáférés-megtagadási üzenetet, győződjön meg arról, hogy a [megfelelő jogosultsági szint](https://docs.microsoft.com/sharepoint/understanding-permission-levels) van hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="c106f-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="c106f-109">**Fontolja meg a hozzáférés-kéra szolgáltatás használatát**</span><span class="sxs-lookup"><span data-stu-id="c106f-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="c106f-110">Az [Access kérelem szolgáltatása](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) lehetővé teszi a felhasználók számára olyan tartalmak elérését, amelyekhez jelenleg nincs engedélyük.</span><span class="sxs-lookup"><span data-stu-id="c106f-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="c106f-111">**Az egyéni parancsfájlok engedélyezhetnek hozzáférés-megtagadási problémákat**</span><span class="sxs-lookup"><span data-stu-id="c106f-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="c106f-112">Vannak olyan helyzetek, amikor az *egyéni parancsfájl engedélyezése* funkció nem engedélyezi a hozzáférés megtagadásáról való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="c106f-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="c106f-113">Az érintett szolgáltatások felsorolása, biztonsági megfontolások és a szolgáltatás letiltásának lehetősége.</span><span class="sxs-lookup"><span data-stu-id="c106f-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="c106f-114">Kérjük, látogasson el az [egyéni parancsfájl engedélyezése vagy tiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="c106f-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

