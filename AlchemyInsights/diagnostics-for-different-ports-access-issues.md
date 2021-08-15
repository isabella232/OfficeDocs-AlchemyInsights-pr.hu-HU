---
title: A különböző portokhoz való hozzáféréssel kapcsolatos problémák diagnosztika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030904"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>A különböző portokhoz való hozzáféréssel kapcsolatos problémák diagnosztika

A különböző portelérési problémák megoldásához végezze el az alábbi lépéseket:

1. A virtuális gép (VM) leállítása/deallocate a portálról, indítsa újra a VM-et, és tesztelje újra. 
2. A VM hálózati beállításait ellenőrizve állapítsa meg, hogy vannak-e hálózati biztonsági csoportok, amelyek letiltják a forgalmat. A Network [Watcher IP-forgalom](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) ellenőrző eszközével is ellenőrizheti, hogy vannak-e olyan NSG-k, amelyek letiltják a forgalmat, a User-Defined Útvonalak (UDRs) a forgalmat a helyszíni környezetbe (0.0.0.0/0/0) vagy egy hálózati készülékhez irányítják vissza.
Ha a fenti lépések után is problémákat tapasztal, kérjük, adja meg a VM nevét és azt a TCP-portot, amelyről levelet próbál küldeni további probléma esetén.

**Ajánlott dokumentumok**

[Korlátozások és javaslatok a 25-ös porton keresztüli kimenő e-mailek küldésére](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)