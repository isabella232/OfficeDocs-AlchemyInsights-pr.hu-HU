---
title: A Yammer rendszergazdákról
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2021
ms.locfileid: "51036715"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="2c5a0-102">A Yammer rendszergazdákról</span><span class="sxs-lookup"><span data-stu-id="2c5a0-102">About Yammer admins</span></span>

<span data-ttu-id="2c5a0-103">**Hálózati rendszergazdák**</span><span class="sxs-lookup"><span data-stu-id="2c5a0-103">**Network admins**</span></span>

<span data-ttu-id="2c5a0-104">A globális rendszergazdákat a rendszer automatikusan igazolt rendszergazdai szerepkörbe lépteti elő egy Yammer hálózatban.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="2c5a0-105">A következő esetekben előfordulhat, hogy a promóció nem megfelelően történik:</span><span class="sxs-lookup"><span data-stu-id="2c5a0-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="2c5a0-106">Több Yammer hálózat is létezik, és a rendszergazda nem a megfelelő hálózatba jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="2c5a0-107">[A hálózat összesítése](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) szükséges ahhoz, hogy egy Yammer meg.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="2c5a0-108">Az Azure PIM használatban van.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-108">Azure PIM is being used.</span></span> <span data-ttu-id="2c5a0-109">Előfordulhat, hogy a felhasználó nem lesz elég ideig előléptetve globális rendszergazdára a promóció bekövetkeztéhez.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="2c5a0-110">A probléma megoldásához Yammer frissítéssel, de a legjobb, ha manuálisan előlépteti a felhasználókat globális rendszergazdára.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="2c5a0-111">Létezik szinkronizálási probléma a Yammer hálózaton.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="2c5a0-112">Ebben az esetben támogatási kérelemre lesz szükség a további vizsgálathoz.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="2c5a0-113">A rendszergazdai szerepkörökről Yammer a Rendszergazdák [Yammer című témakörben.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)</span><span class="sxs-lookup"><span data-stu-id="2c5a0-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="2c5a0-114">**Csoport-rendszergazdák**</span><span class="sxs-lookup"><span data-stu-id="2c5a0-114">**Group admins**</span></span>

<span data-ttu-id="2c5a0-115">A Microsoft 365-hez csatlakoztatott csoportok csoport-rendszergazdái az Azure AD-ból származó csoporttagságokkal vannak szinkronizálva.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="2c5a0-116">Nagy csoportok esetében a szinkronizálás hosszabb ideig is tart.</span><span class="sxs-lookup"><span data-stu-id="2c5a0-116">For large groups, this sync can take an extended period.</span></span>
