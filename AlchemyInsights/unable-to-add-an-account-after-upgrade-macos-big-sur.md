---
title: Nem lehet fiókot hozzáadni a macOS 11.6 Big Sur verzióra való frissítés után
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506479"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Nem lehet fiókot hozzáadni a macOS 11.6 Big Sur verzióra való frissítés után

A macOS 11.6-os verzióra való frissítés után előfordulhat, hogy OneDrive munkahelyi vagy iskolai OneDrive-fiókja, illetve személyes OneDrive-fiókja nem jelenik meg a fiókok listájában, és előfordulhat, hogy nem tud bejelentkezni egy második fiókba az appból.

A problémához már ki van javítva a javítás. Először is állapítsa meg, hogy az appok különálló vagy App Store-beli verzióját OneDrive:

- Válassza OneDrive a felhőt a menüsávon, és > **Súgó & Gépház**  >  **Beállítások about**  >  **elemet.** Ha a verziószám nem tartalmazza a **(Különálló)** verziót, akkor a termék App Store-beli verzióját használja.

Ha az OneDrive különálló verzióját használja, indítsa újra a gépet, OneDrive automatikusan frissül egy olyan buildre, amelyben a probléma megoldódott. Ha manuálisan szeretné telepíteni [a](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)buildet, töltse le ezt az.zip-fájlt, kibontsa a fájlt, és másolja a OneDrive alkalmazást az Alkalmazások mappába (a meglévő OneDrive alkalmazás cseréjével).

Ha az App Store verziót használja, fontolja meg az appok különálló OneDrive. Ez a verzió ugyanúgy működik, mint az App Store verzió, de lehetővé teszi a Microsoftnak, hogy gyorsabban felajánlja a frissítéseket a felhasználóknak, és összekapcsolja őket egy olyan verzióval, amely tartalmazza a probléma megoldását.

1. Töltse le a javítást tartalmazó OneDrive [verzióját.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Unzip the file, and copy the OneDrive app into the Applications folder (by replacing the existing OneDrive app).

Ha az App Store verziót kell használnia, várja meg, amíg az App Store kiadja a javítást tartalmazó appverziót. A Microsoft sajnos nem tudja közölni, hogy egy javított verzió becsült dátumát ki lehet engedni az App Store áruházból.


