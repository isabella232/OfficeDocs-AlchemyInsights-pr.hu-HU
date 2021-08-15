---
title: A Provision szolgáltatás konfigurálása
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
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033280"
---
# <a name="configuring-the-provision-service"></a>A Provision szolgáltatás konfigurálása

Az automatikus felhasználóbeépítéshez az Azure AD-nek érvényes hitelesítő adatokra van szüksége, amelyek lehetővé teszik, hogy csatlakozzon a Workday Web Services API-hoz. Ezenkívül az AD-felhasználó kiépítési apphoz tartozó Workday (Kapcsolat tesztelése) gomb is ellenőrzi, hogy tud-e csatlakozni az AD-tartományhoz társított Azure AD Csatlakozás Provisioning Agent szolgáltatáshoz.

Ha az Azure Portal hibaüzenetet ad vissza a hitelesítő adatok mentésekor, kövesse az alábbi ajánlott lépéseket:

1. Győződjön meg arról, hogy konfigurálta a Workday Integration System User fiókot a [Workdayben](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)című oktatóanyag szakasznak megfelelően.
2. Győződjön meg arról Csatlakozás hogy az Azure AD Csatlakozás Provisioning Agent Szolgáltatás működik-e a helyszíni Windows kiszolgálón a Szolgáltatások kezelése konzol használatával. Az Azure Portalon az ügynök állapotát a Helyszíni ügynökök megtekintése gombra kattintva is ellenőrizheti.
3. Győződjön meg arról, hogy a "Workday Felhasználónév" mező értékét a username@workday-tenant-name formátumban adja meg. Ha hiányzik a workday-tenant-name (munkanap-bérlő neve) hiányzik, a Workday-hitelesítés sikertelen lesz.
4. Ha a Workday-implementáció bérlői fiókkal konfigurálja az integrációt, jegyezze fel a Workday-bérlő ütemezett leállási órákat. A munkabeosztás bérlői webhelyének hétvégekre (általában péntek estétől szombat reggelig) ütemezett leállása, és a leállási időszakban csatlakozási hibák egy ismert probléma, amely automatikusan megoldja a bérlői webhelyet, amint a bérlői webhely újra online állapotba áll.
5. Ritkán előfordulhat az is, hogy ez a hibaüzenet akkor jelenik meg, ha az integrálórendszer-felhasználó jelszava megváltozott a bérlői fiók frissítése miatt, vagy ha a fiók zárolt vagy lejárt állapotban van. Ellenőrizze az integrálórendszer-felhasználó állapotát a Workday rendszergazdájával.

A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további részletekért lásd: Oktatóprogram: A Workday beállítása [automatikus felhasználóbeépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
