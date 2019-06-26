---
title: Teljesítmény problémák SharePoint- vagy OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 9bb18196f38de473e4ee79d77bd43561ad9742e0
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223282"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="53291-102">A SharePoint- vagy OneDrive lassú, nem elérhető vagy nem érhető el, ha több felhasználó</span><span class="sxs-lookup"><span data-stu-id="53291-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="53291-103">Több felhasználó, aki korábban az access OneDrive vagy a SharePoint webhely nem érhető el, ha a szolgáltatás átmeneti probléma lehet.</span><span class="sxs-lookup"><span data-stu-id="53291-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="53291-104">[Ellenőrizze a szolgáltatás egészségügyi irányítópult](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="53291-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="53291-105">**Adjunk hozzá, és a felhasználói licenc**</span><span class="sxs-lookup"><span data-stu-id="53291-105">**Add and license the user**</span></span>

<span data-ttu-id="53291-106">Győződjön meg arról, amikor a [felhasználók az Office 365 rendszerben üzleti licencek hozzárendelése](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="53291-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="53291-107">**Engedélyek hozzárendelése**</span><span class="sxs-lookup"><span data-stu-id="53291-107">**Assign Permissions**</span></span>

<span data-ttu-id="53291-108">Ha a felhasználó Sharepoint licencre van rendelve, és továbbra is a hozzáférés megtagadva üzenetet kap, ellenőrizze, hogy rendelkezik a [megfelelő jogosultsági szint](https://docs.microsoft.com/sharepoint/understanding-permission-levels) hozzárendelt.</span><span class="sxs-lookup"><span data-stu-id="53291-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="53291-109">**Fontolja meg a hozzáférési kérelem szolgáltatás**</span><span class="sxs-lookup"><span data-stu-id="53291-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="53291-110">A [hozzáférési kérelem szolgáltatás](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) segítségével a felhasználók a tartalom megtekintéséhez engedéllyel jelenleg nem rendelkeznek hozzáférést kérni.</span><span class="sxs-lookup"><span data-stu-id="53291-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="53291-111">**Lehetővé teszi egyéni parancsfájl hozzáférés megtagadva problémákat okozhat.**</span><span class="sxs-lookup"><span data-stu-id="53291-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="53291-112">Vannak bizonyos helyzetek, ahol az *egyéni parancsfájlok engedélyezése* a szolgáltatás lehet tárni a hozzáférés megtagadva.</span><span class="sxs-lookup"><span data-stu-id="53291-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="53291-113">Az érintett szolgáltatások listáját, biztonsági megfontolások és képessége, hogy tiltsa le a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="53291-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="53291-114">Látogasson el a [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="53291-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

