---
title: Lemezterület felszabadítja a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036587"
---
# <a name="free-up-drive-space-in-windows-10"></a>Lemezterület felszabadítja a Windows 10-ben

A következő két lehetőséggel szabadíthat fel lemezterületet a Windowsban:

- Szabadíthat fel lemezterületet a Windows 10-ben.
- Tárterületet szabadíthat fel a Windows 10-frissítések számára külső tárolóeszköz segítségével.

Ha a Lemezkarbantartó használata után továbbra is kevés a lemezterület, akkor lehet, hogy a Temp mappa gyorsan kitölti a Microsoft Store által használt alkalmazásfájlokat (.appx). A probléma megoldásához állítsa alaphelyzetbe az Áruházat, ürítse ki az Áruház gyorsítótárát, majd futtassa a Windows Update hibaelhárítót. Mielőtt továbblép, győződjön meg arról, hogy a Microsoft Store be van zárva.

**1. lépés: A Microsoft Store alaphelyzetbe állítása**

**Megjegyzés** Ez véglegesen törli az alkalmazásadatokat az eszközön, beleértve a beállításokat és a bejelentkezési adatokat.

1. Válassza a **Start**  >  **Settings**  >  **Apps apps**&  >  **gombra.**

1. Az appok listájában keresse meg és válassza a Microsoft Store lehetőséget.

1. Válassza **a Speciális beállítások lehetőséget.**

1. Görgessen le, és **válassza az Alaphelyzet**, majd az **Alaphelyzetbe állítás megerősítése lehetőséget.**

**2. lépés: A Microsoft Store gyorsítótárának kiürítése**

1. A Windows billentyű + R billentyűkombinációt lenyomva nyissa meg a Futtatás párbeszédpanelt.

1. Írja be a wsreset.exe, és válassza az **OK gombot.**

1. Megnyílik egy üres parancssorablak. Körülbelül 10 másodperc elteltével az ablak bezárul, és az Áruház automatikusan megnyílik.

**3. lépés: A Windows Update alaphelyzetbe állítása**

1. Válassza **a Start**  >  **Settings** Update & Biztonsági hibaelhárítás  >    >  **lehetőséget.**

1. Görgessen le, és válassza a **Windows Update** listában a Hibaelhárító **futtatása lehetőséget.**

1. Indítsa újra a számítógépet, és ellenőrizze, hogy továbbra is tapasztalja-e a problémát.

