---
title: Megjegyzések listaelemekhez
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982491"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="d9b0a-102">Megjegyzések listaelemekhez</span><span class="sxs-lookup"><span data-stu-id="d9b0a-102">Comments on List items</span></span>

<span data-ttu-id="d9b0a-103">A felhasználók hamarosan hozzáadhatnak és törölhetnek megjegyzéseket a listaelemekhez.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="d9b0a-104">A felhasználók megtekinthetik a listaelemek minden megjegyzését, és szűrhetik az egy elemhez kapcsolódó megjegyzéseket vagy tevékenységeket megjelenítő nézetek között.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="d9b0a-105">**Időzítés** :</span><span class="sxs-lookup"><span data-stu-id="d9b0a-105">**Timing** :</span></span>

<span data-ttu-id="d9b0a-106">**Célzott kiadás** : fokozatos kilépés az októberi közép-és első lépésekkel – november közepéig</span><span class="sxs-lookup"><span data-stu-id="d9b0a-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="d9b0a-107">**Szokásos kiadás** : fokozatos Kilépés a novemberi közép-és a decemberi első lépésekkel</span><span class="sxs-lookup"><span data-stu-id="d9b0a-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="d9b0a-108">**Bevezetés** : célzott kiadás a teljes szervezet számára</span><span class="sxs-lookup"><span data-stu-id="d9b0a-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="d9b0a-109">A felhasználóknak a megjegyzések hozzáadásához és törléséhez a következőket kell megjegyezniük:</span><span class="sxs-lookup"><span data-stu-id="d9b0a-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="d9b0a-110">A megjegyzések a SharePointban rejlő jogosultsági beállításokat követik.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="d9b0a-111">A modern felhasználói felületeken, például a feladatlistákban még nem megjelenő klasszikus listák nem fogják tartalmazni a megjegyzések hozzáfűzését.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="d9b0a-112">Ebben a kiadásban nem érhető el megjegyzések a Teams listáihoz.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="d9b0a-113">A megjegyzéseket a keresés nem indexeli.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="d9b0a-114">A rendszergazdák a **set-SPOTenant PowerShell-** parancsmagban a **CommentsOnListItemsDisabled** paraméter módosításával letilthatják ezt a funkciót szervezeti szinten.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="d9b0a-115">A webhely vagy a lista szintjén jelenleg nem lehet letiltani a megjegyzéseket.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="d9b0a-116">Reméljük, hogy ezeket a vezérlőket egy későbbi frissítésben, az 2021 első negyedévében kell megnyitnia.</span><span class="sxs-lookup"><span data-stu-id="d9b0a-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
