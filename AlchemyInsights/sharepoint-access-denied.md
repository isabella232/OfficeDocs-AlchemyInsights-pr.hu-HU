---
title: A hozzáférés megtagadva üzenetet – problémamegoldás
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: a8eb435e9e19d1c5bcdb694b899e09a4126b8697
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761191"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="87b5e-102">A hozzáférés megtagadva üzenetet – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="87b5e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="87b5e-103">Ha a hozzáférés megtagadásáról a Sharepoint Online webhely böngészése közben kap, olvassa el az alábbi cikkek.</span><span class="sxs-lookup"><span data-stu-id="87b5e-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="87b5e-104">**Adjunk hozzá, és a felhasználói licenc**</span><span class="sxs-lookup"><span data-stu-id="87b5e-104">**Add and License the user**</span></span>

<span data-ttu-id="87b5e-105">Győződjön meg arról, amikor a [felhasználók az Office 365 rendszerben üzleti licencek hozzárendelése](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="87b5e-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="87b5e-106">**Engedélyek hozzárendelése**</span><span class="sxs-lookup"><span data-stu-id="87b5e-106">**Assign Permissions**</span></span>

<span data-ttu-id="87b5e-107">Ha a felhasználó Sharepoint licencre van rendelve, és továbbra is a hozzáférés megtagadva üzenetet kap, ellenőrizze, hogy rendelkezik a [megfelelő jogosultsági szinthez tartozó](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="87b5e-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="87b5e-108">**Fontolja meg a hozzáférési kérelem szolgáltatás**</span><span class="sxs-lookup"><span data-stu-id="87b5e-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="87b5e-109">Az [access-request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) szolgáltatás lehetővé teszi a tartalom megtekintéséhez engedéllyel jelenleg nem rendelkeznek hozzáférési kérelmek emberek.</span><span class="sxs-lookup"><span data-stu-id="87b5e-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="87b5e-110">**Lehetővé teszi egyéni parancsfájl hozzáférés megtagadva problémákat okozhat.**</span><span class="sxs-lookup"><span data-stu-id="87b5e-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="87b5e-111">Vannak bizonyos esetek, ahol az "Egyéni parancsfájl engedélyezése" szolgáltatás lehet tárni a hozzáférés megtagadva.</span><span class="sxs-lookup"><span data-stu-id="87b5e-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="87b5e-112">Az érintett szolgáltatások listáját, biztonsági megfontolások és képessége, hogy tiltsa le a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="87b5e-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="87b5e-113">Látogasson el a, [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="87b5e-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="87b5e-114">Megjegyzés: Ha több felhasználónak, aki korábban a hozzáférést a OneDrive vagy a SharePoint webhely nem érhető el, lehet egy ideiglenes szolgáltatást a probléma.</span><span class="sxs-lookup"><span data-stu-id="87b5e-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="87b5e-115">[Ellenőrizze a szolgáltatás egészségügyi irányítópult](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="87b5e-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

