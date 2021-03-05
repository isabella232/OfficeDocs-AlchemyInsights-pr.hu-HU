---
title: Az AD-felhasználó kiépítési munkanapja karanténba kerül
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481876"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Az AD-felhasználó kiépítési munkanapja karanténba kerül

**Az AD-felhasználó kiépítési munkanapja karanténba kerül, és nem jön létre felhasználó az AD-ban**

Az AD-felhasználó kiépítési feladata karanténba került, és a naplók az exportálási hibák eseményeit mutatják a következő **hibaüzenettel: OperationsError-SvcErr: Művelethiba történt. A címtárszolgáltatáshoz nincs konfigurálva felsőbbrendű hivatkozás. A címtárszolgáltatás ezért nem tud** az erdőn kívüli objektumokra hivatkozni. Ez a hiba általában akkor jelenik meg, ha az Active Directory-tároló szervezeti egység nincs megfelelően beállítva, vagy ha problémák vannak a **parentDistinguishedName** kifejezésleképezésével kapcsolatban.

Ellenőrizze, hogy az Új felhasználók alapértelmezett felhasználói **felhasználóinak** paramétere nem-e elkallokokat. Győződjön meg arról, hogy a megadott szervezeti egység már szerepel az AD-ben. Ha a **parentDistinguishedName** értéket használja az attribútumleképezésben, gondoskodjon arról, hogy az mindig egy ismert tároló legyen az AD tartományon belül. A létrehozott érték megtekintéséhez ellenőrizze az Exportálás eseményt a naplókban.

A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további információkért lásd: A Munkanap beállítása automatikus felhasználói [kiépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

