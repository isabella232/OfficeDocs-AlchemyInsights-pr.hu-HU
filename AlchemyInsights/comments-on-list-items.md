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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724156"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="6a736-102">Megjegyzések listaelemekhez</span><span class="sxs-lookup"><span data-stu-id="6a736-102">Comments on List items</span></span>

<span data-ttu-id="6a736-103">A felhasználók megtekinthetik a listaelemek minden megjegyzését, és szűrhetik az egy elemhez kapcsolódó megjegyzéseket vagy tevékenységeket megjelenítő nézetek között.</span><span class="sxs-lookup"><span data-stu-id="6a736-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="6a736-104">A felhasználóknak a megjegyzések hozzáadásához és törléséhez a következőket kell megjegyezniük:</span><span class="sxs-lookup"><span data-stu-id="6a736-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="6a736-105">A megjegyzések a SharePointban rejlő jogosultsági beállításokat követik.</span><span class="sxs-lookup"><span data-stu-id="6a736-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="6a736-106">A modern felhasználói felületeken, például a feladatlistákban még nem megjelenő klasszikus listák nem fogják tartalmazni a megjegyzések hozzáfűzését.</span><span class="sxs-lookup"><span data-stu-id="6a736-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="6a736-107">Ebben a kiadásban nem érhető el megjegyzések a Teams listáihoz.</span><span class="sxs-lookup"><span data-stu-id="6a736-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="6a736-108">A megjegyzéseket a keresés nem indexeli.</span><span class="sxs-lookup"><span data-stu-id="6a736-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="6a736-109">A rendszergazdák a **set-SPOTenant PowerShell-** parancsmagban a **CommentsOnListItemsDisabled** paraméter módosításával letilthatják ezt a funkciót szervezeti szinten.</span><span class="sxs-lookup"><span data-stu-id="6a736-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="6a736-110">A webhely vagy a lista szintjén jelenleg nem lehet letiltani a megjegyzéseket.</span><span class="sxs-lookup"><span data-stu-id="6a736-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="6a736-111">Reméljük, hogy ezeket a vezérlőket egy későbbi frissítésben, az 2021 első negyedévében kell megnyitnia.</span><span class="sxs-lookup"><span data-stu-id="6a736-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
