---
title: Endpoint Manager – Biztonsági alaptervek
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923556"
---
# <a name="endpoint-manager---security-baselines"></a>Endpoint Manager – Biztonsági alaptervek

A biztonsági alaptervek előre konfigurált Windows beállítások csoportja, amelyek segítenek Önnek alkalmazni azokat a beállításokat, amelyet a releváns biztonsági csoportok ajánlottak. Ezeket az alapterveket testre lehet szabni, hogy csak a kívánt beállításokat és értékeket adják vissza. További információkért a biztonsági alaptervekről, lásd a [Biztonsági alaptervek használata a Windows 10 eszközök Intune-ban való konfigurálásához](https://docs.microsoft.com/mem/intune/protect/security-baselines)menüpontot.

Jelenleg ezekhez a termékekhez találhatók alaptervek:

- Windows MDM Biztonsági beállítások
- Végponthoz készült Microsoft Defender Biztonság
- Microsoft Edge

Mindegyik alaptervet időszakosan frissítjük és lépésenkénti verziókban adjuk ki. Mindegyik verzió hozzáad, vagy eltávolít beállításokat az előző verziókból annak érdekében, hogy az alapterv az aktuális útmutatásnak megfelelő legyen. A Biztonsági alapterv konzolja a Végpont biztonságban lehetővé teszi a különböző verziók összehasonlítását azáltal, hogy láthatóvá teszi a verziónkénti változtatásokat.

Ahhoz az útmutatáshoz, hogy leghatékonyabban lehessen módosítani, melyik alapterv van üzembe helyezve, lásd a [Biztonsági alapterv-profilok kezelése a Microsoft Intune-ban](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure) lehetőséget.

A biztonsági alapterv üzemebe helyezése után megfigyelheti az üzembe helyezés állapotát és áttekintheti a beállításokat eszközről eszközre.

Mivel a biztonsági alapértékek számos beállítást tartalmaznak, fontos áttekinteni a konfigurációs módosításokat, és tesztelni, hogy az összes beállítás megfelelő legyen az eszközeihez és az üzleti igényeihez.

**Megjegyzés:** Az alaptervek jelentési adatának megjelenése akár 24 órát is igénybe vehet az eszközre való telepítés előkészítésétől, és akár 6 órát is a további frissítéseknél. 

A leggyakoribb oka annak, ha egy alapterv-beállítás nem alkalmazható az, hogy ugyanazt a beállítást már egy másik profilban is használják. Bizonyos eszköznél ki lehet vizsgálni ezt a forgatókönyvet a Biztonsági alapterv profiljának Eszközállapot csomópontjából. További részletekért lásd a [Biztonsági alaptervek konfliktusainak megoldása](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines) menüpontot.