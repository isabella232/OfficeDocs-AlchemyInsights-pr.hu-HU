---
title: EndPoint Manager – Biztonsági alapértékek
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420881"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – Biztonsági alapértékek

A biztonsági alapértékek a Windows beállításainak előre konfigurált csoportjai, amelyek segítenek a megfelelő biztonsági csoportok által ajánlott biztonsági beállítások alkalmazásában. Ezek az alapértékek testre szabhatók úgy, hogy csak a kívánt beállításokat és értékeket adjanak eredményre. A biztonsági alapértékekkel kapcsolatos további információkért lásd: Windows 10-es eszközök konfigurálása biztonsági alaptervekkel [az Intune-ban.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Ezekhez a termékekhez jelenleg alapértékek vannak:

- A Windows MDM biztonsági beállításai
- Microsoft Defender az EndPoint biztonságért
- Microsoft Edge

Az alaptervek egyesét rendszeres időközönként frissítjük, és növekményes verziókban adva ki. Minden egyes verzió hozzáadja és eltávolítja az előző verzió beállításait, hogy az alapterv megfeleljen az aktuális útmutatásnak. Az Endpoint Security Security Alaptervek konzolja lehetővé teszi a különböző verziók összehasonlítását úgy, hogy láthatóvá teszi a verzióról verzióra vonatkozó módosításokat.

Ha segítségre van szüksége ahhoz, hogy a leghatékonyabban módosítsa az alapterv verzióját, tekintse meg az Alapterv biztonsági profilok kezelése a [Microsoft Intune-ban](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Egy biztonsági alapterv telepítése után eszközönként figyelheti a központi telepítés állapotát, és áttekintheti a beállításokat.

**Megjegyzés:** Az alaptervek jelentéskészítési adatai akár 24 órát is igénybe vehetnek a kezdeti telepítéstől az eszközig, illetve akár 6 órát is igénybe vehetnek a további frissítések. 

Az alapterv-beállítások alkalmazásának leggyakoribb oka az, hogy ugyanazt a beállítást használják egy másik profilban. Az adott eszközre vonatkozó eset megvizsgálása az Alap biztonsági alapterv profil Eszköz állapota csomópontján lehetséges. Részletes információkért lásd: [Ütközések feloldása biztonsági alaptervek esetén.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)