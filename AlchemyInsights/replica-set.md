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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110682"
---
# <a name="replica-set"></a>Replikakészlet

Az AADDS-t felügyelt tartománynak is nevezik. Valójában két tartományvezérlőt kell futtatni és karbantartani a háttérkiszolgálón. A két DCS egy fő tartományvezérlőt és egy replikációs DC-t tartalmaz. Az AADDS (felügyelt tartomány) biztonsági másolatai az Azure platform által kezelt automatizált folyamat. Ha probléma ad problémát a felügyelt tartománnyal kapcsolatban, az Azure ügyfélszolgálata segíthet a biztonsági mentésből való visszaállításban.

Minden replikakészletet egy virtuális hálózatban hozhat létre. Minden virtuális hálózatnak társviszonyban kell lennie minden más olyan virtuális hálózattal, amely a felügyelt tartomány replikakészletét kezeli. Ez a konfiguráció hálóhálózati topológiát hoz létre, amely támogatja a címtár-replikációt. A virtuális hálózatok több replikakészletet is támogatnak, feltéve, hogy minden replikakészlet egy másik virtuális alhálózatban található.

A Replikakészletről további információt a [Koncepciók](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)replikakészletek .
