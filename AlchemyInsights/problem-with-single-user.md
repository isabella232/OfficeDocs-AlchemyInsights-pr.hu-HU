---
title: Probléma egyetlen felhasználóval
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960153"
---
# <a name="problem-with-single-user"></a>Probléma egyetlen felhasználóval

- Előfordulhat, hogy a felhasználó nem lett kiépítve, mert a szolgáltatásnak még nem volt lehetősége kiértékelni a felhasználót. Tekintse át az útmutatót arról, hogy mennyi ideig tart a kiépítés, valamint a kiépítési konfigurációs lap folyamatjelző sávja. Ha a további részletek szakaszban meghatározott egyenletes állapot a felhasználó létrehozási/frissítési/törlési dátuma előtt áll, az azt jelenti, hogy még nem értékeltük ki a felhasználót. Ebben az esetben a legjobb megoldás, ha megvárja, amíg a kiépítési szolgáltatás befejeződik.

  - Felhívjuk a figyelmét arra, hogy szolgáltatásunk csak a forrásrendszerben (felhőbeli HR) felhasználó módosításairól tud. A forrásrendszerben érvényes változásnak kell lennie ahhoz, hogy az Azure AD észlelje a változást, és átfolyatja azt az Active Directoryba.
- A kiépítési szolgáltatás kiértékelte a felhasználót, és megállapította, hogy azt nem kell kiépítenünk:
  - Ha attribútumalapú hatókör-szűrést adott meg, ellenőrizze, hogy a felhasználó megfelel-e az Ön által megadott feltételeknek.
  - Ha a felhasználók már léteznek a célrendszerben, és a felhasználó állapota a forrás- és célértékben egyezésben van, akkor nem tudunk további lépéseket.
- A kiépítési szolgáltatás megkísérli kiépítni a felhasználót, és az nem sikerült. Ilyen esetekben tekintse át a kiépítési naplók hibaelhárítási és javaslatok lapját:
  - Előfordulhat, hogy a felhasználó egy kötelező attribútuma hiányzik a helyszíni Active Directoryból vagy az Azure AD-ből. A userPrincipalName vagy az sAMAccountName generációs szabályok például nem a megfelelő értéket generálják.
  - Az egyező attribútum (általában employeeId) nem ad feloldása egy egyedi felhasználónak a helyszíni Active Directoryban vagy az Azure AD-ban. Tegyük fel például, hogy két felhasználónak ugyanaz az alkalmazottazonosítója az AD szolgáltatásban, és a szolgáltatás egy hibaüzenetet ad vissza, amely ugyanazt a forrásbejegyzést duplikált célbejegyzésként jelzi.

Az egyes felhasználók és csoportok naplóit az Adott felhasználóval kapcsolatos probléma kiépítési naplóiban olvassa [el.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
