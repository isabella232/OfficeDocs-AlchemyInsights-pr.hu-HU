---
title: 0x8004de40 hiba a OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946581"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 hiba a OneDrive

Ha hibaüzenet jelenik meg, **0x8004de40** a OneDrive, indítsa újra a számítógépet, miközben a munkahelyi vagy iskolai tartományhoz csatlakozik. Ha az újraindítás után a következő hibaüzenet jelenik meg, próbálkozzon ezzel a munkahelyi vagy iskolai tartományhoz való csatlakozáskor:

1. Kattintson a Start gombra, írja be a **cmd** vagy **a parancssor** parancsot a keresőmezőbe, kattintson a jobb gombbal a parancssor alkalmazásra, és válassza a **Futtatás rendszergazdaként parancsot.** Ha a rendszer rendszergazdai jelszó vagy megerősítés kérését kéri, írja be a jelszót, vagy kattintson az Allow (Megengedve) **gombra.**  

2. A Parancssor ablakban írja be a **dsregcmd /leave**  parancsot, és várja meg, amíg befejeződik a parancs. Ezután írja be a **dsregcmd /join parancsot,** és várja meg, amíg befejeződik a parancs.
3. Indítsa újra a számítógépet.
