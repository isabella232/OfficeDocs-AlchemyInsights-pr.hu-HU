---
title: Teljesítménnyel kapcsolatos problémák–SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511150"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a3122-102">A SharePoint vagy a OneDrive lassú, nem elérhető vagy több felhasználó számára nem érhető el</span><span class="sxs-lookup"><span data-stu-id="a3122-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="a3122-103">Ha egy OneDrive- vagy SharePoint-webhely nem érhető el több olyan felhasználó számára, akinek korábban hozzáférése volt, előfordulhat, hogy ideiglenes szolgáltatásprobléma lépett fel.</span><span class="sxs-lookup"><span data-stu-id="a3122-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a3122-104">[Ellenőrizze a szolgáltatás állapotának irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="a3122-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="a3122-105">**A felhasználó hozzáadása és licencelése**</span><span class="sxs-lookup"><span data-stu-id="a3122-105">**Add and license the user**</span></span>

<span data-ttu-id="a3122-106">Győződjön meg arról, [hogy licenceket rendel a Microsoft 365 vállalati verzió felhasználóihoz.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="a3122-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="a3122-107">**Engedélyek hozzárendelése**</span><span class="sxs-lookup"><span data-stu-id="a3122-107">**Assign Permissions**</span></span>

<span data-ttu-id="a3122-108">Ha a felhasználó sharepoint-licencet kapott, és továbbra is megtagadott hozzáférési üzenetet kap, győződjön meg arról, hogy rendelkezik a [megfelelő jogosultsági szinttel.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="a3122-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="a3122-109">**Fontolja meg a hozzáférési kérelem szolgáltatás használatát**</span><span class="sxs-lookup"><span data-stu-id="a3122-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="a3122-110">A [hozzáférés-kérelem funkció](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) lehetővé teszi, hogy a személyek olyan tartalomhoz kérjenek hozzáférést, amelynek megtekintéséhez jelenleg nincs engedélye.</span><span class="sxs-lookup"><span data-stu-id="a3122-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="a3122-111">**Az egyéni parancsfájl engedélyezése a hozzáférés megtagadási problémáit okozhatja**</span><span class="sxs-lookup"><span data-stu-id="a3122-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="a3122-112">Vannak bizonyos esetek, ahol az *egyéni parancsfájl engedélyezése* szolgáltatás lehet bemutató hozzáférés megtagadva.</span><span class="sxs-lookup"><span data-stu-id="a3122-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="a3122-113">Az érintett szolgáltatások listájához biztonsági szempontok és a szolgáltatás letiltásának lehetősége.</span><span class="sxs-lookup"><span data-stu-id="a3122-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a3122-114">Kérjük, látogasson el [az Egyéni parancsfájl engedélyezése vagy megakadályozása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="a3122-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

