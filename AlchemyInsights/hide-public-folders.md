---
title: Nyilvános mappák elrejtése
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315372"
---
# <a name="hide-public-folders"></a>Nyilvános mappák elrejtése

**A teljes nyilvános mappafa elrejtése:**

A cikkben található [lépésekkel](https://aka.ms/ControlPF) teljes nyilvános mappafát rejthet el a szelektív vagy az összes felhasználó elől.

**Adott nyilvános mappa elrejtése:**

1. Engedélyek hozzáadása a nyilvános mappához hozzáféréssel rendelkező felhasználóknak

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Távolítsa el az **alapértelmezett felhasználót** az **engedélylistából:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
