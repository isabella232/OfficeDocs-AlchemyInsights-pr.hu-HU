---
title: Teams nem indul el
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813349"
---
# <a name="teams-doesnt-launch"></a>Teams nem indul el

Ha megpróbál megnyitni egy Microsoft Teams de nem indul el, próbálkozzon az alábbiakkal:

1. Tallózással keresse meg **az %appdata%\Microsoft\Teams.**
1. Törölje a mappa tartalmát.
1. Indítsa újra a számítógépet, és próbálja meg elindítani a Teams.

Előfordulhat, hogy újra kell telepítenie a Teams. Újratelepítés:

1. Távolítsa Teams a Vezérlőpulttal.
1. Tallózással keresse meg **az %appdata%\Microsoft\Teams\Application Cache mappáját.**
1. Törölje a mappa tartalmát.
1. Tallózással keresse meg **az %appdata%\Microsoft\teams\Cache adatokat.**
1. Törölje a mappa tartalmát.
1. Indítsa újra a számítógépet, majd töltse le és telepítse Teams.

Ha a bérlői fiókban egy olyan felhasználó diagnosztikai eszközét szeretné futtatni, aki nem tud bejelentkezni, indítson új keresést a **TeamsUserUnableToSignIn** kulcsszóval, és kövesse az utasításokat.