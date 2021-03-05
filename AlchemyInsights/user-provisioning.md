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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481889"
---
# <a name="user-provisioning"></a>Felhasználó kiépítése

- Az [igény szerinti](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) kiépítési funkcióval kiépíti a felhasználót, és részletes diagnosztikai adatokat kap a szükséges lépésekről.
- A felhasználók és csoportok kiépítésekor felmerülő hibák elhárításához tekintse meg a hibaelhárítási útmutatót, amely során nem történik felhasználók [kiépítése.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Ha megfigyeli, hogy a felhasználók nincsenek kiépítve, tekintse meg a kiépítési naplókat [(előzetes verzió)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) az Azure Active Directoryban (AD). Adott felhasználóhoz tartozó naplóbejegyzések keresése
- Rendszeres időközönként indítsa újra a kiépítést az előző kiépítési ciklusban kihagyott felhasználók elfogása érdekében.
- Előfordulhat, hogy a felhasználó/csoport nem lett kiépítve, mert a szolgáltatásunknak még nem volt lehetősége kiértékelni a felhasználót. Tekintse át az útmutatót, hogy mennyi ideig tart a kiépítés, valamint a kiépítési konfigurációs lap folyamatjelző sávja. Ha a további részletek szakaszban megadott egyenletes állapot a felhasználó létrehozási/frissítés/törlési dátuma előtt áll, az azt jelenti, hogy még nem értékeltük ki a felhasználót. Ebben az esetben a legjobb, ha megvárja, amíg befejeződik a kiépítési szolgáltatás. Ha egyenletes állapot érhető el, javasoljuk, hogy indítsa újra az Azure Portal felhasználói felületét.
  - Felhívjuk a figyelmét arra, hogy szolgáltatásunk csak a forrásrendszerben (Azure Active Directory) lévő felhasználók/csoportok módosításait ismeri. Ha egy felhasználót vagy csoportot közvetlenül az alkalmazásból távolít el (például a ServiceNow szolgáltatást), nem tudunk a változásokról, és a forrásrendszerben a felhasználó állapota alapján nem áll vissza. Ebben az esetben a legjobb, ha közvetlenül a célalkalmazásban visszaveszi a változtatást.
- Szolgáltatásunk kiértékelte a felhasználót/csoportot, és megállapította, hogy nem szükséges kiépítenünk:
  - Ha beállította a hatókört a hozzárendelt felhasználókra és csoportokra, ellenőrizze, hogy a felhasználó/csoport hozzá van-e rendelve az alkalmazáshoz.
  - Ha a felhasználó/csoport hozzá van rendelve az alkalmazáshoz, győződjön meg arról, hogy nincs hozzárendelve az alapértelmezett hozzáférési szerepkörhöz. Ez a szerepkör nem használható kiépítésre.
  - Ha beállított egy attribútumalapú hatókör-szűrési szűrőt, győződjön meg arról, hogy a felhasználó megfelel az Ön által megadott feltételeknek.
  - Ha a felhasználók már léteznek a célrendszerben, és a felhasználó állapota a forrás- és cél egyezésben, nem tudunk semmilyen további műveletet.
- Szolgáltatásunk megkísérelte kiépítni a felhasználót, és az nem sikerült. Ilyen esetekben tekintse át a kiépítési naplók hibaelhárítási és javaslatok lapját:
  - Előfordulhat, hogy a felhasználó egy kötelező attribútuma hiányzik az Azure Active Directoryból, vagy nem felel meg a külső alkalmazás által megkövetelt formátumnak. Előfordulhat például, hogy egy felhasználó Ország attribútuma az Amerikai Egyesült Államokra van állítva, amikor az Amerikai Egyesült Államoknak kell lennie.
  - Az attribútum egy hivatkozási attribútum, amely még nem létezik a célalkalmazásban. A hivatkozási attribútum egy attribútum, amely egy másik objektumra mutat, például egy csoport tagja. A felhasználó azonosítója a csoport tagattribútumában lenne, de csak akkor feldolgozható, ha az a felhasználói objektum, amelyre mutat, már létezik.
