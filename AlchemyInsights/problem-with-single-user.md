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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429715"
---
# <a name="problem-with-single-user"></a>Probléma egyetlen felhasználóval

- Előfordulhat, hogy a felhasználó nem lett kiépítve, mert a szolgáltatásnak még nem volt lehetősége kiértékelni a felhasználót. Tekintse át az útmutatót, hogy mennyi ideig tart a kiépítés, valamint a kiépítési konfigurációs lap folyamatjelző sávja. Ha a további részletek szakaszban megadott egyenletes állapot a felhasználó létrehozási/frissítés/törlési dátuma előtt áll, az azt jelenti, hogy még nem értékeltük ki a felhasználót. Ebben az esetben a legjobb, ha megvárja, amíg befejeződik a kiépítési szolgáltatás.

  - Felhívjuk a figyelmét arra, hogy szolgáltatásunk csak a forrásrendszerben (felhőbeli HR) felhasználó módosításait ismeri. Az Azure AD-nek érvényes változásnak kell lennie a forrásrendszerben ahhoz, hogy észlelje a változást, és átfolyta azt az Active Directoryba.
- A kiépítési szolgáltatás kiértékelte a felhasználót, és megállapította, hogy nem szükséges kiépítve:
  - Ha beállított egy attribútumalapú hatókör-szűrési szűrőt, győződjön meg arról, hogy a felhasználó megfelel az Ön által megadott feltételeknek.
  - Ha a felhasználók már léteznek a célrendszerben, és a felhasználó állapota a forrás- és cél egyezésben, nem tudunk semmilyen további műveletet.
- A kiépítési szolgáltatás megkísérelte kiépítni a felhasználót, és az nem sikerült. Ilyen esetekben tekintse át a kiépítési naplók hibaelhárítási és javaslatok lapját:
  - Előfordulhat, hogy a felhasználó egy kötelező attribútuma hiányzik a helyszíni Active Directoryból vagy az Azure AD-ből. A userPrincipalName vagy sAMAccountName generációs szabályok például nem a megfelelő értéket generálják.
  - Az egyező attribútum (általában employeeId) nem megoldás egy egyedi felhasználónál a helyszíni Active Directoryban vagy az Azure AD-ban. Két felhasználónak például ugyanaz az alkalmazottazonosítója van az AD-ban, és a szolgáltatás hibaüzenetet ad vissza, amely ugyanazt a forrásbejegyzést jelzi duplikált célbejegyzésként.

Az egyes felhasználók és csoportok naplóit a kiépítési naplók áttekintése egy adott felhasználóval kapcsolatos [problémához olvassa el.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
