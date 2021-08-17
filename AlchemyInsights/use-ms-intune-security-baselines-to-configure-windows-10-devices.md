---
title: Az Microsoft Intune biztonsági alapértékek használatával konfigurálhatja Windows 10 eszközöket
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104346"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Az Microsoft Intune biztonsági alapértékek használatával konfigurálhatja Windows 10 eszközöket

Az Intune biztonsági alaptervei segítenek megvédeni a felhasználókat és az eszközöket. A biztonsági alapértékek Windows beállítások előre konfigurált csoportjai, amelyek az adott biztonsági csoportok által ajánlott ismert beállítások és alapértelmezett értékek alkalmazásával használhatók. Ha létrehoz egy alapterv biztonsági profilt az Intune-ban, olyan sablont hoz létre, amely több eszközkonfigurációs profilból áll.

Amikor biztonsági alapterveket telepít felhasználók vagy eszközök csoportjain vagy eszközein, a beállításokat a rendszer az Windows 10 vagy újabb eszközökön alkalmazza. Az automatikus mobileszköz-biztonsági alapérték (1) például engedélyezi a BitLockert a cserélhető meghajtókon, (2) jelszóra van szükség az eszköz zárolásának feloldásához, és (3) letiltja az alapvető hitelesítést. Ha egy alapértelmezett érték nem működik a környezetben, testre szabhatja az alaptervet a szükséges beállítások alkalmazásához.

A biztonsági alapértékek egy végpontok közötti biztonságos munkafolyamatot is Microsoft 365. Az alábbiakban ennek néhány előnye van:

- A biztonsági alapértékek a biztonságot befolyásoló beállításokhoz ajánlott eljárásokat és javaslatokat tartalmaznak. Mivel az Intune a Windows biztonsági csapatával, amely alapértékeket hoz létre a csoportházirendek számára, ezek a javaslatok megbízható útmutatáson és kiterjedt tapasztalaton alapulnak.
- Ha ön az Intune új felhasználója, és nem tudja, hol kezdje, akkor a biztonsági alapértékek segítségével gyorsan létrehozhat és üzembe helyezhet egy biztonságos profilt.
- Ha jelenleg csoportházirendet használ, akkor a biztonsági alapértékekkel sokkal egyszerűbb az Intune-ra való áttelepítés, mivel ezek beépítve vannak az Intune-ba, és élvonalbeli funkciókat tartalmaznak a kezeléshez.

További információt a [](https://go.microsoft.com/fwlink/?linkid=2141503) Biztonsági alapértékek Windows mobileszköz-kezelés [– útmutatóban olvashat.](https://go.microsoft.com/fwlink/?linkid=2141701)