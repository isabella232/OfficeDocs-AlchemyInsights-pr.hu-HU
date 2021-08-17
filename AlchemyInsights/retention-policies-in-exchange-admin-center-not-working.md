---
title: Az Adatmegőrzési házirendek Exchange Felügyeleti központban nem működik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074934"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Adatmegőrzési házirendek Exchange Felügyeleti központban

Ha azt szeretné, hogy automatikusan ellenőrizjük az alább említett beállításokat, válassza a vissza gombot < - a lap tetején, majd adja meg annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az adatmegőrzési házirendekkel.

Ha problémákat tapasztal az adatmegőrzési házirendekkel a Exchange Felügyeleti központban nem vonatkoznak az archív postaládába át nem indító postaládákra vagy elemekre, ellenőrizze az alábbiakat:

**A probléma gyökerének okai:**

- **A Felügyeltmappa-segéd** nem feldolgozta a felhasználó postaládáját. A Felügyeltmappa-segéd hét naponta egyszer próbálja feldolgozni a felhőalapú szervezet összes postaládáját.

  **Megoldás:** Futtassa a Felügyeltmappa-segédet.

- **A RetentionHold** engedélyezve **van a** postaládában. Ha a postaláda Adatmegőrzési Visszatartás helyen van, a postaládára vonatkozó adatmegőrzési házirend feldolgozása ez idő alatt nem történik meg.

  **Megoldás:** Ellenőrizze az Adatmegőrzési visszatartás beállítás állapotát, és szükség szerint frissítse azt. További részleteket a Postaláda-megőrzési [visszatartás .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Megjegyzés:** Ha egy postaláda 10 MB-nál kisebb méretű, a Felügyeltmappa-segéd nem fogja automatikusan feldolgozni a postaládát.
 
Az adatmegőrzési házirendek a Felügyeleti központban Exchange további információkért lásd:

- [Adatmegőrzési címkék és adatmegőrzési házirendek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Adatmegőrzési házirend alkalmazása postaládákra](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) vagy [Adatmegőrzési címkék hozzáadása vagy eltávolítása](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [A postaláda típusú visszatartott szöveg azonosítása](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
