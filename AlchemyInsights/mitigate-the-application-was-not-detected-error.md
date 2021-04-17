---
title: A Nem sikerült észlelni az alkalmazást hiba előfordulásainak csökkentése
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836353"
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
