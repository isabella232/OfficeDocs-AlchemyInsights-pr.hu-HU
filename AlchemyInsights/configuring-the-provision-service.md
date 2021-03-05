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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482869"
---
# <a name="configuring-the-provision-service"></a>A Provision szolgáltatás konfigurálása

A felhasználók automatikus kiépítése csak akkor működik, ha az Azure AD érvényes hitelesítő adatokkal rendelkezik, amelyek lehetővé teszik, hogy csatlakozzon a Workday Web Services API-hoz. A Workday to AD User Provisioning app Tesztkapcsolat gombja ezenkívül ellenőrzi, hogy képes-e csatlakozni az AD-tartományhoz társított Azure AD Connect Provisioning Agent szolgáltatáshoz.

Ha az Azure Portal hibaüzenetet ad vissza a hitelesítő adatok mentésekor, kövesse az alábbi ajánlott lépéseket:

1. Ellenőrizze, hogy konfigurálta-e a Workday Integration System felhasználói fiókját a Workday alkalmazás integrációs rendszerének felhasználóit ismertető oktatóanyag [szakaszának megfelelően.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Győződjön meg arról, hogy az Azure AD Connect Provisioning Agent szolgáltatás a szolgáltatások felügyeleti konzolját használva működik a helyszíni Windows-kiszolgálón. Az Azure Portalon az ügynök állapotát a Helyszíni ügynökök megtekintése gombra kattintva is ellenőrizheti.
3. Győződjön meg arról, hogy a "Workday Username" mező értékét az username@workday-tenant-name formátumban adja meg. Ha a munkanap-bérlő-név hiányzik, a Workday-hitelesítés sikertelen lesz.
4. Ha a Workday implementációs bérlői fiókkal konfigurálja az integrációt, jegyezze fel a Workday-bérlő ütemezett állásidejét. A munkabeosztási bérlők leállását a hétvégékre (általában péntek estétől szombat reggelig) ütemezte, és a leállási időkeret csatlakozási sikertelenségei ismert problémát jelentek, amely automatikusan megoldja a problémát, amint a bérlők újra online állapotba állnak.
5. Ritkán ez a hibaüzenet akkor is előfordulhat, ha az integrálórendszer-felhasználó jelszava megváltozott a bérlői fiók frissítése miatt, vagy ha a fiók zárolt vagy lejárt állapotban van. Ellenőrizze az integrációs rendszer felhasználójának állapotát a Workday rendszergazdájával.

A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további információkért lásd: A Munkanap beállítása automatikus felhasználói [kiépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
