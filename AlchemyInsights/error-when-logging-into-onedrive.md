---
title: 0x8004de40 hiba az OneDrive indításakor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823050"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 hiba az OneDrive indításakor

Ha hibaüzenet jelenik meg, amikor bejelentkezik a OneDrive-ba, indítsa újra a számítógépet a munkahelyi vagy iskolai tartományhoz való **0x8004de40** . Ha az újraindítás után a következő hibaüzenet jelenik meg, próbáljon meg csatlakozni a munkahelyi vagy iskolai tartományához:

1. Kattintson a Start gombra, és írja be a **cmd** vagy a **parancssor**  kifejezést a keresőmezőbe, kattintson a jobb gombbal a parancssor alkalmazásra, és válassza a  **Futtatás rendszergazdaként** parancsot. Ha a rendszer rendszergazdai vagy megerősítési jelszót kér, írja be a jelszót, vagy kattintson az **Engedélyezés** gombra.  

2. A parancssorablakban írja be a **dsregcmd/Leave**  , és várjon, amíg meg nem jelenik a parancs. Ezután írja be a **dsregcmd/JOIN** , és várja meg, amíg a parancs el nem fejeződik.
3. Indítsa újra a számítógépet.
