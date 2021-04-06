---
title: Lemezterület felszabadítása a Windows 10 rendszerben
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505358"
---
# <a name="free-up-drive-space-in-windows-10"></a>Lemezterület felszabadítása a Windows 10 rendszerben

Alább bemutatunk két lehetőséget arra, hogyan szabadíthat fel lemezterületet a Windowsban:

- Felszabadíthat lemezterületet a Windows 10-ben.
- Külső tárolóeszköz segítségével felszabadíthat tárterületet a Windows 10 frissítései számára.

Ha a Lemezkarbantartó használata után is kevés a szabad lemezterület, előfordulhat, hogy a Temp mappában gyorsan összegyűlnek a Microsoft Store által használt alkalmazásfájlok (.appx). A probléma elhárításához állítsa alaphelyzetbe a Store-t, ürítse ki a Store gyorsítótárát, majd futtassa a Windows Update hibaelhárítóját. Ügyeljen arra, hogy az alábbi lépések elvégzése előtt bezárja a Microsoft Store-t.

**1. lépés: A Microsoft Store alaphelyzetbe állítása**

**Megjegyzés:** Ez a művelet véglegesen törli az eszközön levő alkalmazásadatokat, beleértve a személyes beállításokat és a bejelentkezési adatokat is.

1. Válassza a **Start** > **Gépház** > **Alkalmazások** > **Alkalmazások és szolgáltatások** lehetőséget.

1. Keresse meg és jelölje ki a Microsoft Store-t az alkalmazások listáján.

1. Válassza a **Speciális beállítások** lehetőséget.

1. Görgessen lefelé, és válassza az **Alaphelyzet** gombot, majd a felugró panelen válassza ismét az **Alaphelyzet** gombot.

**2. lépés: A Microsoft Store gyorsítótárának kiürítése**

1. Nyomja le a Windows billentyűt + az R billentyűt a Futtatás párbeszédpanel megnyitásához.

1. Írja be a wsreset.exe parancsot, és válassza az **OK** gombot.

1. Ekkor megnyílik egy üres parancssori ablak. Körülbelül 10 másodperc elteltével az ablak bezárul, és automatikusan megnyílik a Store.

**3. lépés: A Windows Update alaphelyzetbe állítása**

1. Válassza a **Start** > **Gépház** > **Frissítés és biztonság** > **Hibaelhárítás** lehetőséget.

1. Görgessen lefelé, és jelölje ki a lista **Windows Update** elemét, majd válassza **A hibaelhárító futtatása** gombot.

1. Indítsa újra a számítógépet, és ellenőrizze, hogy továbbra is tapasztalja-e a problémát.

