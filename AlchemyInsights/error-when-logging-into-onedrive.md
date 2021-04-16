---
title: 0x8004de40 OneDrive indításakor hibaüzenet jelenik meg
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813654"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 OneDrive indításakor hibaüzenet jelenik meg

Ha hibaüzenet jelenik meg, **0x8004de40** OneDrive-ba való bejelentkezéskor, indítsa újra a számítógépet, miközben a munkahelyi vagy iskolai tartományhoz csatlakozik. Ha az újraindítás után a következő hibaüzenet jelenik meg, próbálkozzon ezzel a munkahelyi vagy iskolai tartományhoz való csatlakozáskor:

1. Kattintson a Start gombra, írja be a **cmd** vagy **a parancssor** parancsot a keresőmezőbe, kattintson a jobb gombbal a parancssor alkalmazásra, és válassza a **Futtatás rendszergazdaként parancsot.** Ha a rendszer rendszergazdai jelszó vagy megerősítés kérését kéri, írja be a jelszót, vagy kattintson az Allow (Megengedve) **gombra.**  

2. A Parancssor ablakban írja be a **dsregcmd /leave**  parancsot, és várja meg, amíg befejeződik a parancs. Ezután írja be a **dsregcmd /join parancsot,** és várja meg, amíg befejeződik a parancs.
3. Indítsa újra a számítógépet.
