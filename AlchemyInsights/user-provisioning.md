---
title: Felhasználó kiépítése
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971341"
---
# <a name="user-provisioning"></a>Felhasználó kiépítése

- Az igény [szerinti kiépítési](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) funkcióval kiépít egy felhasználót, és részletes diagnosztikát kap a lépésekről.
- A felhasználók és csoportok kiépítésekor felmerülő hibák elhárításához tekintse meg a hibaelhárítási útmutatóT: [Nincs kiépítve felhasználó.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Ha megfigyeli, hogy a felhasználók nincsenek kiépítve, tekintse meg a [provisioning logs (preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD). Adott felhasználóhoz tartozó naplóbejegyzések keresése
- Rendszeres időközönként indítsa újra a kiépítést az előző kiépítési ciklusban kihagyott felhasználók ki elfogása érdekében.
- Előfordulhat, hogy a felhasználó/csoport nem lett kiépítve, mert a szolgáltatásunknak még nem volt lehetősége kiértékelni a felhasználót. Tekintse át az útmutatót arról, hogy mennyi ideig tart a kiépítés, valamint a kiépítési konfigurációs lap folyamatjelző sávja. Ha a további részletek szakaszban meghatározott egyenletes állapot a felhasználó létrehozási/frissítési/törlési dátuma előtt áll, az azt jelenti, hogy még nem értékeltük ki a felhasználót. Ebben az esetben a legjobb megoldás, ha megvárja, amíg a kiépítési szolgáltatás befejeződik. Ha egyenletes állapot érhető el, javasoljuk, hogy indítsa újra az Azure Portal felhasználói felületét.
  - Felhívjuk a figyelmét arra, hogy szolgáltatásunk csak a forrásrendszerben (felhasználói/csoportban) végrehajtott Azure Active Directory. Ha egy felhasználót/csoportot közvetlenül az alkalmazásból távolít el (például ServiceNow), akkor nem tudunk a változásokról, és a forrásrendszerben a felhasználó állapota alapján nem állunk vissza. Ebben az esetben a legjobb, ha közvetlenül a célalkalmazásban visszaveszi a változtatást.
- Szolgáltatásunk kiértékelte a felhasználót/csoportot, és úgy határozott, hogy nem szükséges kiépítenünk:
  - Ha beállította a hatókört felhasználók és csoportok hozzárendelésére, ellenőrizze, hogy a felhasználó/csoport hozzá van-e rendelve az alkalmazáshoz.
  - Ha a felhasználó/csoport hozzá van rendelve az alkalmazáshoz, győződjön meg arról, hogy nincsenek hozzárendelve az alapértelmezett hozzáférési szerepkörhöz. Ez a szerepkör nem használható kiépítésre.
  - Ha attribútumalapú hatókör-szűrést adott meg, ellenőrizze, hogy a felhasználó megfelel-e az Ön által megadott feltételeknek.
  - Ha a felhasználók már léteznek a célrendszerben, és a felhasználó állapota a forrás- és célértékben egyezésben van, akkor nem tudunk további lépéseket.
- Szolgáltatásunk megkísérli kiépítni a felhasználót, és az nem sikerült. Ilyen esetekben tekintse át a kiépítési naplók hibaelhárítási és javaslatok lapját:
  - Előfordulhat, hogy a felhasználó kötelező attribútuma hiányzik Azure Active Directory vagy nem felel meg a külső alkalmazás által megkövetelt formátumnak. Előfordulhat például, hogy egy felhasználó Country attribútuma az Amerikai Egyesült Államokban van beállítva, ha az US.
  - Az attribútum egy olyan hivatkozási attribútum, amely még nem létezik a célalkalmazásban. A hivatkozási attribútum egy olyan attribútum, amely egy másik objektumra, például egy csoport tagja egy felhasználóra mutat. A felhasználó azonosítója a csoport tagattribútumában lenne, de csak akkor feldolgozható, ha az objektum, amelyre mutat, már létezik.
