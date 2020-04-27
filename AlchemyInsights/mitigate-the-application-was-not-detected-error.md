---
title: A Nem sikerült észlelni az alkalmazást hiba előfordulásainak csökkentése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810486"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>A „Nem sikerült észlelni az alkalmazást” hiba előfordulásainak csökkentése

Az Intune által jelentett „Nem sikerült észlelni az alkalmazást a telepítés sikeres befejezése után” alkalmazástelepítési hiba az összes fontos operációs rendszeren (Windows, iOS és Android) jelentkezhet.

A hibát kiváltó leggyakoribb esetek közé tartoznak a következők:

- A kezdeti rendszerbe állítást követően az Intune-on kívül frissítették az alkalmazást (harmadik fél alkalmazás-áruházából). Előfordulhat például, hogy bizonyos alkalmazások – mint például a Google Chrome – automatikus frissítéseket hajtanak végre.
- Egy felhasználó eltávolította az alkalmazást annak kezdeti telepítése után.

A probléma megoldásához először ellenőrizze az érintett eszközöket, hogy megállapíthassa, melyik eset vezet a hibához.

- Ha az Intune-on kívül frissítették az alkalmazást, akkor az alkalmazás üzemeltetése beállítható úgy, hogy figyelmen kívül hagyja az alkalmazás verziószámát. Ehhez állítsa **Igen** értékre az **Alkalmazás konfigurációja > Alkalmazásadatok** csoportban levő **Alkalmazás verziójának figyelmen kívül hagyása** beállítást.
- Az ügyfél célzásakor célszerű lehet „kötelező” módon telepíteni az alkalmazást, és biztosítani, hogy a legújabb verzió legyen rendszerbe állítva.
- Az iOS platformon azt is megteheti, hogy az Apple mennyiségi vásárlási programjához társított **automatikus frissítési** funkciót használja, amely konfigurálható úgy, hogy automatikusan frissítsen az új alkalmazásverziókra, amint azok elérhetővé válnak.

Az alkalmazások telepítésével kapcsolatos hibák elhárításáról az [Alkalmazástelepítési problémák elhárítása](https://docs.microsoft.com/intune/troubleshoot-app-install) című témakörben olvashat bővebben.
