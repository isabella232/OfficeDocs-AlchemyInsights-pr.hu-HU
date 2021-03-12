---
title: Replikakészlet
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714248"
---
# <a name="replica-set"></a>Replikakészlet

Az AADDS-t felügyelt tartománynak is nevezik. Valójában két tartományvezérlőt futtat és tart fenn a háttérkiszolgáló. A két DCs egy fő tartományvezérlőt és egy replikációs tartományvezérlőt tartalmaz. Az AADDS (felügyelt tartomány) biztonsági másolatai az Azure platform által kezelt automatizált folyamatok. Ha probléma ad problémát a felügyelt tartománnyal, az Azure ügyfélszolgálata segítséget nyújthat a biztonsági másolatból való visszaállításban.

Minden egyes replikakészletet egy virtuális hálózaton hozhat létre. Minden virtuális hálózatnak társviszonyban kell lennie minden más olyan virtuális hálózattal, amely a felügyelt tartomány replikakészletét kezeli. Ez a konfiguráció hálóhálózati topológiát hoz létre, amely támogatja a címtár-replikációt. A virtuális hálózatok több replikakészletet is támogatnak, feltéve, hogy minden egyes replikakészlet egy másik virtuális alhálózatban található.

A Replikakészlettel kapcsolatos további információkért lásd [a "Concepts Replikakészletek" halmazt.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
