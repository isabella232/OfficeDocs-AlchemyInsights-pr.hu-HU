---
title: Hálózati vizsgálat letiltása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7e67a45b6f4d4b18f47ce55a0fde20f826498c5d25c4a6dec4311d8fe4c3735f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928551"
---
# <a name="disable-network-scan"></a>Hálózati vizsgálat letiltása

A hálózati megosztáson való vizsgálat hatással lehet a teljesítményre.  Ha meg kell győződni arról, hogy az ügyfél alapértelmezés szerint nem olvassa át a hálózati megosztásokat/fájlokat, állítsa az alábbi beállításokat a Windows Defender alkalmazásban True **(Igaz) beállításra:**

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles