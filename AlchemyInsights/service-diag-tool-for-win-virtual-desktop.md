---
title: Service diagnostics tool for Windows Virtual Desktop
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052388"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service diagnostics tool for Windows Virtual Desktop

Windows A Virtual Desktop (WVD) diagnosztikai eszközével a rendszergazdák egyetlen felületen azonosíthatja a hibákat. Ez az eszköz diagnosztikai adatokat naplóz minden alkalommal, amikor egy WVD-szerepkörrel társított felhasználó használja a WVD-et. Minden napló tartalmazza a tevékenységben érintett WVD szerepkört, a munkamenet során megjelenő hibaüzeneteket, valamint a bérlő és a felhasználó adatait. Az Azure Log Analytics konfigurálható a diagnosztikai eszköz által létrehozott tevékenységnapló rögzítésére. Ezt a következőképpen teheti meg:

1. Hozzon létre egy Log Analytics munkaterületet az [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) vagy a [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Csatlakozás Windows át a számítógépeket az Azure Monitor alkalmazásba.](https://go.microsoft.com/fwlink/?linkid=2129913) Szerezze be a munkaterület azonosítóját és a munkaterület elsődleges kulcsát. A beállítási varázslónak szüksége van erre az információra, hogy megfelelően konfigurálja az ügynököt, és biztosítsa, hogy képes legyen kommunikálni az Azure Monitorral.
1. [Leküldéses diagnosztikai adatok a munkaterületre.](https://go.microsoft.com/fwlink/?linkid=2128284) Leküldéses diagnosztikai adatokat a WVD-bérlőről a munkaterület naplóelemzésébe.
1. [A WVD-vel](https://go.microsoft.com/fwlink/?linkid=2128338) kapcsolatos belső vagy külső problémák azonosítása és diagnosztizálása.

A szolgáltatásdiagnosztikai eszköz WVD-hez való konfigurálásával kapcsolatos további információkért lásd: A diagnosztikai funkció használata [a naplóelemzéssel.](https://go.microsoft.com/fwlink/?linkid=2128084)
