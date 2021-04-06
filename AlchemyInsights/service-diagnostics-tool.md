---
title: Service diagnostics tool for Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595869"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service diagnostics tool for Windows Virtual Desktop

A Windows Virtual Desktop (WVD) diagnosztikai eszközével a rendszergazdák egyetlen felületen azonosíthatja a hibákat. Ez az eszköz diagnosztikai adatokat naplóz minden alkalommal, amikor egy WVD-szerepkörrel társított felhasználó használja a WVD-et. Minden napló tartalmazza a tevékenységben érintett WVD szerepkört, a munkamenet során megjelenő hibaüzeneteket, valamint a bérlő és a felhasználó adatait. Az Azure Log Analytics konfigurálható a diagnosztikai eszköz által létrehozott tevékenységnapló rögzítésére az alábbi lépésekkel:

1. Hozzon létre egy Log Analytics munkaterületet az [Azure Portal vagy](https://go.microsoft.com/fwlink/?linkid=2129500) az Azure [PowerShell segítségével.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Windows rendszerű számítógépek csatlakoztatása az Azure Monitorhoz.](https://go.microsoft.com/fwlink/?linkid=2129913) Szerezze be a munkaterület azonosítóját és a munkaterület elsődleges kulcsát. A beállítási varázslónak szüksége van erre az információra, hogy megfelelően konfigurálja az ügynököt, és biztosítsa, hogy képes legyen kommunikálni az Azure Monitorral.

1. [Leküldéses diagnosztikai adatok a munkaterületre.](https://go.microsoft.com/fwlink/?linkid=2128284) Leküldéses diagnosztikai adatokat a WVD-bérlőről a munkaterület naplóelemzésébe.

1. [A](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) WVD-vel kapcsolatos belső vagy külső problémák azonosítása és diagnosztizálása.

A szolgáltatásdiagnosztikai eszköz WVD-hez való konfigurálásával kapcsolatos további információkért lásd: A diagnosztikai funkció használata a naplóelemzéssel.