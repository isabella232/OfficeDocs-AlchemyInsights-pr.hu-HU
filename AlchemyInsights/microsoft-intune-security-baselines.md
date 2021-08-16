---
title: Az Microsoft Intune biztonsági alapértékek használatával konfigurálhatja Windows 10 eszközöket
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 0a89b121f2f425b0a81fa250650f108e9af48c9da39dfc8a62b07541d3a6c3dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098064"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Az Microsoft Intune biztonsági alapértékek használatával konfigurálhatja Windows 10 eszközöket

Az Intune biztonsági alaptervei segítenek megvédeni a felhasználókat és az eszközöket. A biztonsági alapértékek Windows beállítások, amelyek az adott biztonsági csoportok által ajánlott ismert beállítások és alapértelmezett értékek alkalmazásával előre megadott csoportokra vonatkoznak. Ha létrehoz egy alapterv biztonsági profilt az Intune-ban, olyan sablont hoz létre, amely több eszközkonfigurációs profilból áll.

Amikor biztonsági alapterveket telepít felhasználók vagy eszközök csoportjain vagy eszközein, a beállításokat a rendszer az Windows 10 vagy újabb eszközökön alkalmazza. A Microsoft mobileszköz-kezelés (MDM) biztonsági alapterve például automatikusan engedélyezi a BitLockert a cserélhető meghajtókon, megköveteli az eszköz zárolásának feloldásához szükséges jelszót, és letiltja az alapvető hitelesítést. Ha egy alapértelmezett érték nem működik a környezetben, testre szabhatja az alaptervet a szükséges beállítások alkalmazásához.

A biztonsági alapértékek egy végpontok közötti biztonságos munkafolyamatot is Microsoft 365. A biztonsági alapértékek a biztonságot befolyásoló beállításokhoz ajánlott eljárásokat és javaslatokat tartalmaznak. Intune-partnerek a Windows biztonsági csapatával, amely alapértékeket hoz létre a csoportházirendek számára, így ezek az ajánlások megbízható útmutatáson és kiterjedt tapasztalaton alapulnak.

Ha most először hozza létre az Intune-t, és nem tudja, hol kezdje, a biztonsági alapértékek segítségével gyorsan létrehozhat és üzembe helyezhet egy biztonságos profilt. Ha jelenleg csoportházirendet használ, a biztonsági alapértékekkel sokkal egyszerűbb az Intune-ra való áttelepítés, mivel ezek az Intune beépített kezelési lehetőségei.

További információt a [](/windows/security/threat-protection/windows-security-baselines) Biztonsági alapértékek Windows mobileszköz-kezelés [– útmutatóban olvashat.](/windows/client-management/mdm/)

