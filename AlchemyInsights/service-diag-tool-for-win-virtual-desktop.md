---
title: A Windows Virtual Desktop szolgáltatás diagnosztikai eszköze
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678622"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>A Windows Virtual Desktop szolgáltatás diagnosztikai eszköze

A Windows Virtual Desktop (WVD) diagnosztikai eszköz segítségével a rendszergazdák egyetlen felületen azonosíthatják a hibákat. Ez az eszköz diagnosztikai információkat naplóz, ha a WVD a WVD szerepkört hozzárendelt valaki használja. Az egyes naplók információkat tartalmaznak a tevékenységben részt vevő WVD szerepről, a munkamenet során megjelenő hibaüzenetekről, valamint a bérlőről és a felhasználóról szóló információkról. Az Azure log Analytics beállítható úgy, hogy a diagnosztikai eszköz által létrehozott műveletnapló rögzítse a naplót. Ezt a következőképpen teheti meg:

1. Hozzon létre egy log Analytics-munkaterületet az [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) vagy az [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)segítségével.
1. [Windows-számítógépek csatlakoztatása az Azure monitorhoz](https://go.microsoft.com/fwlink/?linkid=2129913). A munkaterület-azonosító és a munkaterület elsődleges kulcsának beszerzése. A beállítási varázslónak szüksége van erre az információra az ügynök megfelelő konfigurálásához és az Azure monitorral való kommunikációhoz.
1. [A diagnosztika adatainak leküldése a munkaterületre](https://go.microsoft.com/fwlink/?linkid=2128284). A diagnosztikai adatait lenyomhatja a WVD-bérlőtől a munkaterülete log-elemzéséhez.
1. [Azonosíthatja és diagnosztizálhatja](https://go.microsoft.com/fwlink/?linkid=2128338) az WVD kapcsolatos belső vagy külső problémákat.

Ha többet szeretne tudni a WVD szolgáltatás diagnosztikai eszközének konfigurálásáról, olvassa el [a naplózási elemzés használata a diagnosztikai szolgáltatáshoz](https://go.microsoft.com/fwlink/?linkid=2128084)című témakört.
