---
title: Felügyeleti egységmegoldás
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7896"
ms.openlocfilehash: c32d0652642fa4143b037662809f3ca5dec079f0
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885061"
---
# <a name="administrative-unit-solution"></a><span data-ttu-id="f99e7-102">Felügyeleti egységmegoldás</span><span class="sxs-lookup"><span data-stu-id="f99e7-102">Administrative unit solution</span></span>

1. <span data-ttu-id="f99e7-103">Győződjön meg arról, hogy a felügyeleti egységeket és a szerepkörök hozzárendelését használó felhasználó globális rendszergazda vagy jogosultsági szerepkör-rendszergazda.</span><span class="sxs-lookup"><span data-stu-id="f99e7-103">Ensure that the user creating the administrative units and assigning roles is a global administrator or a privilege role administrator.</span></span>
2. <span data-ttu-id="f99e7-104">Győződjön meg arról, hogy közvetlenül a felügyeleti egységekhez rendeli hozzá a felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="f99e7-104">Ensure you are assigning users directly to the administrative units.</span></span> <span data-ttu-id="f99e7-105">Ha egy csoportot hozzárendel egy felügyeleti egységhez, az nem rendeli hozzá a csoport összes tagját a felügyeleti egységhez.</span><span class="sxs-lookup"><span data-stu-id="f99e7-105">Assigning a group to an administrative unit does not assign all the members of the group to the administrative unit.</span></span>
3. <span data-ttu-id="f99e7-106">A felügyeleti egységeken végrehajtott tömeges művelet esetén a módosítások a különféle tényező(k) (például aktuális szolgáltatásbetöltés) függvényében a felhasználói felületen való tükrözéshez is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="f99e7-106">For a bulk operation performed on an administrative unit, the changes may take time to reflect in the UI, depending on various factor(s) such as current service load.</span></span>

<span data-ttu-id="f99e7-107">A felügyeleti egységekről további információt a Szerepkörök kezelése a Felügyeleti [egységben.](https://docs.microsoft.com/azure/active-directory/roles/administrative-units)</span><span class="sxs-lookup"><span data-stu-id="f99e7-107">For more details about administrative units, see [Manage roles in Administrative unit](https://docs.microsoft.com/azure/active-directory/roles/administrative-units).</span></span>
