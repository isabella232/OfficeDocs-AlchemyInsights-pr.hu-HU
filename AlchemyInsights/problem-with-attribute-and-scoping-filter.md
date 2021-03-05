---
title: Probléma az attribútum- és hatókör-szűrési szűrővel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481892"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Probléma az attribútum- és hatókör-szűrési szűrővel

**Probléma az ütköző UPN-értékekkel**

The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.** A művelet nem sikerült, mert az összeadáshoz/módosításhoz megadott UPN-érték nem egyedi erdőszintű. Hiba részletei: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

Az **a userPrincipalName érték,** amit a Workday-összekötő próbál beállítani az AD felhasználói fiók létrehozásakor, már létezik a cél AD tartományban. Ez azt jelenti, hogy vagy (1) már létezik a felhasználó, és az egyező azonosító ellenőrzése sikertelen volt a felhasználónál, vagy (2) az UPN-generációs szabály ütköző értéket generált.

Íme a javasolt megoldási lépések:

Ha a felhasználó már létezik, és a megfelelő azonosító-ellenőrzés nem tudta összekapcsolni a Workday-fiókot az Active Directory-fiókkal, akkor ellenőrizze, hogy a Workday és az AD azonosítójának egyező attribútuma (jellemzően **employeeID)** pontosan egyezik-e. Ha nincs egyezésük, azt az adat problémáját kell kijavítanunk. Ha például a Workday alkalmazottazonosítója 001052, az AD-ben pedig 1052, akkor a kiépítési motor nem tudja összekapcsolni a két fiókot, és megpróbál létrehozni egy már létező felhasználót. Ebben az esetben úgy kell  módosítania az Alkalmazottazonosító értékét az AD-ben, hogy az tartalmazza a kezdő nullákat, hogy 001052 legyen.
Ha az UPN-et generáló kifejezés nem hoz létre egyedi értéket, érdemes lehet a **SelectUniqueValue** duplikálásának függvényével minden alkalommal egyedi értéket létrehozni.

**Az AD-felhasználó kiépítésének munkanapja nem ad meg kezelői attribútumértéket az AD-felhasználói fiókhoz**

Az AD-felhasználó kiépítési feladata nem  a kezelő attribútumértékének beállítása az AD-felhasználói fiókokhoz. Ennek a viselkedésnek két lehetséges forgatókönyve van:

1. A Workdayben a vezető nem oldható fel egy megfelelő AD-felhasználói fiókkal, mert a vezető nincs hatókörben.
2. Több **AD-tartomány** esetén a Workday kezelője nem ugyanabban a tartományban van, mint a felhasználó.

A probléma megoldásához próbálkozzon az alábbi lépésekkel:

1. Ha hatókör-meghatározási szűrőket definiált, először ellenőrizze, hogy a kezelő hatóköre kiterjed-e, és hogy megfelel-e a hatókör-meghatározási záradéknak. Ha a vezető nem felel meg a hatókör-szűrési szűrőnek, módosítsa úgy a szűrőt, hogy a kezelő a kiépítési művelet hatókörében is kiterjedni.
2. Ha több AD-tartománya van, akkor az összekötőben ismert korlátozás van, hogy nem lehet feloldani a tartományközi kezelői hivatkozásokat.

A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további információkért lásd: A Munkanap beállítása automatikus felhasználói [kiépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













