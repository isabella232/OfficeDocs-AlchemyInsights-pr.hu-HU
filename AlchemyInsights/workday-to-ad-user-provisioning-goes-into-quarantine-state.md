---
title: Workday to AD User Provisioning goes into quarantine state
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
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036494"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday to AD User Provisioning goes into quarantine state

**Az AD-felhasználó kiépítési munkanapja karanténba kerül, és nem jön létre felhasználó az AD-ban**

Az AD-felhasználó kiépítési feladata karanténba került, és a naplók az exportálási hibák eseményeit mutatják a következő **hibaüzenettel: OperationsError-SvcErr: Művelethiba történt. Nincs beállítva felsőbbrendű hivatkozás a címtárszolgáltatáshoz. A címtárszolgáltatás ezért nem tud** ajánlást ki kibocsátásra az erdőn kívüli objektumokhoz. Ez a hiba általában akkor jelenik meg, ha az Active Directory-tároló szervezeti egység nincs megfelelően beállítva, vagy ha problémák vannak a **parentDistinguishedName** kifejezésleképezésével kapcsolatban.

Ellenőrizze, hogy nincs-e elkallálás az Új felhasználók alapértelmezett felhasználóinak paraméterrel.  Győződjön meg arról, hogy a megadott szervezeti egység már szerepel az AD-ben. Ha a **parentDistinguishedName** értéket használja az attribútumleképezésben, gondoskodjon arról, hogy az mindig egy ismert tároló legyen az AD-tartományon belül. A létrehozott érték megtekintéséhez jelölje be az Esemény exportálása a naplókban jelölőnégyzetet.

A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további részletekért lásd: Oktatóprogram: A Workday beállítása [automatikus felhasználóbeépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

