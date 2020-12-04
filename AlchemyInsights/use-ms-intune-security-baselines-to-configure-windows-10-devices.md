---
title: Windows 10-es eszközök beállítása a Microsoft Intune biztonsági alaptervek segítségével
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573540"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Windows 10-es eszközök beállítása a Microsoft Intune biztonsági alaptervek segítségével

Az Intune biztonsági alaptervek segítenek megvédeni a felhasználókat és az eszközöket. A biztonsági alaptervek a Windows-beállítások előre konfigurált csoportjai, amelyek a beállítások ismert csoportját és a megfelelő biztonsági csoportok által javasolt alapértelmezett értékeket alkalmazzák. Ha az Intune-ban biztonsági alapprofilokat hoz létre, több eszköz-konfigurációs profilból álló sablont hoz létre.

Ha a biztonsági alapterveket felhasználók vagy eszközök csoportjaiba telepíti, a beállítások a Windows 10 vagy újabb rendszerű eszközökön érvényesek. Például a MDM biztonsági alapterv automatikusan (1) engedélyezi a BitLocker használatát a cserélhető meghajtókon (2) az eszközök zárolásának feloldásához, és (3) letiltja az egyszerű hitelesítést. Ha egy alapértelmezett érték nem működik a környezetében, az alapterv testreszabásával alkalmazza a szükséges beállításokat.

A biztonsági alaptervek a Microsoft 365-ban is segítenek az end-to-end biztonsági munkafolyamatok létrehozásában. Az alábbi előnyök a következők:

- Egy biztonsági alapterv tartalmazza a biztonsági beállításokat érintő gyakorlati tanácsokat és javaslatokat. Mivel az Intune partnerei a Windows biztonsági csapata alapterveket hoz létre a csoportházirendekhez, ezek az ajánlások a Solid Orientációs és a széleskörű használatot szolgálják.
- Ha nem biztos abban, hogy hol találja meg az Intune-t, és nem biztos abban, hogy hol találja meg a kezdést, a biztonsági alaptervek segítségével gyorsan létrehozhat és üzembe helyezhet egy biztonságos profilt.
- Ha jelenleg egy csoportházirendet használ, akkor az Intune felügyeleti célokra való áttelepítése jóval megkönnyíti a biztonsági alaptervek használatát, mivel ezek a felhasználók a Intune szolgáltatásba kerülnek, és magukban foglalják a kezelés élvonalbeli funkcióit.

További információt a [Windows biztonsági alaptervek](https://go.microsoft.com/fwlink/?linkid=2141503) és a [mobileszköz-kezelés](https://go.microsoft.com/fwlink/?linkid=2141701)című témakörben találhat.