---
title: A Microsoft Intune biztonsági alaptervek használata a Windows 10-es eszközök beállításához
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694433"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>A Microsoft Intune biztonsági alaptervek használata Windows 10-es eszközök konfigurálásához

Az Intune biztonsági alaptervei segítenek megvédeni a felhasználókat és az eszközöket. A biztonsági alapértékek a Windows beállításainak olyan előre konfigurált csoportjai, amelyek a megfelelő biztonsági csoportok által ajánlott ismert beállításokat és alapértelmezett értékcsoportokat alkalmazzák. Ha létrehoz egy alapbiztonsági profilt az Intune-ban, több eszközkonfigurációs profilból áll egy sablon.

Amikor biztonsági alapértékeket telepít felhasználók vagy eszközök csoportjaira, a beállítások a Windows 10-es vagy újabb verzióin futó eszközökre vonatkoznak. A Microsoft mobileszköz-kezelési (MDM) biztonsági alapterve például automatikusan (1) engedélyezi a BitLocker használatát a cserélhető meghajtókhoz, (2) az eszköz zárolásának feloldásához szükséges jelszót, és (3) letiltja az alapszintű hitelesítést. Ha egy alapértelmezett érték nem működik a környezetben, testre szabhatja az alaptervet a szükséges beállítások alkalmazásához.

A biztonsági alapértékek szintén segítenek a végpontok közötti biztonságos munkafolyamatok létrehozására a Microsoft 365-ben. Az alábbiakban a funkció néhány előnyét kínáljuk:
- A biztonsági alapértékek a biztonságot befolyásoló beállításokhoz ajánlott eljárásokat és javaslatokat tartalmaznak. Mivel az Intune partneri viszonyban van a Windows biztonsági csapatával, amely alapterveket hoz létre a csoportházirendek számára, ezek a javaslatok megbízható útmutatáson és kiterjedt felhasználói élményen alapulnak.
- Ha még nem tudja, hogy hol kezdje az Intune-t, akkor a biztonsági alapértékek segítségével gyorsan létrehozhat és üzembe helyezhet egy biztonságos profilt.
- Ha jelenleg csoportházirendet használ, akkor a biztonsági alapértékekkel sokkal egyszerűbb az Intune-ra való áttelepítés, mivel ezek a biztonsági alapértékek az Intune beépített funkciói, és a kezelés élvonalbeli funkcióival rendelkeznek.

További információt a Windows biztonsági [alaptervei és](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [a Mobileszköz-kezelés.](https://docs.microsoft.com/windows/client-management/mdm/)