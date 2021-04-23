---
title: Nem működnek az adatmegőrzési házirendek az Exchange Felügyeleti központban
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952230"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Adatmegőrzési házirendek az Exchange Felügyeleti központban

Ha azt szeretné, hogy automatikusan ellenőrizjük az alább említett beállításokat, válassza a vissza gombot < - a lap tetején, majd adja meg annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az adatmegőrzési házirendekkel.

Ha az Exchange Felügyeleti központban az adatmegőrzési házirendek nem vonatkoznak olyan postaládákra vagy elemekre, amelyek nem az archív postaládába vonatkoznak, ellenőrizze az alábbiakat:

**A probléma gyökerének okai:**

- **A Felügyeltmappa-segéd** nem feldolgozta a felhasználó postaládáját. A Felügyeltmappa-segéd hét naponta egyszer próbálja feldolgozni a felhőalapú szervezet összes postaládáját.

  **Megoldás:** Futtassa a Felügyeltmappa-segédet.

- **A RetentionHold** engedélyezve **van a** postaládában. Ha a postaláda Adatmegőrzési Visszatartás helyen van, a postaládára vonatkozó adatmegőrzési házirend feldolgozása ez idő alatt nem történik meg.

  **Megoldás:** Ellenőrizze az Adatmegőrzési visszatartás beállítás állapotát, és szükség szerint frissítse azt. További részleteket a Postaláda-megőrzési [visszatartás .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Megjegyzés:** Ha egy postaláda 10 MB-nál kisebb méretű, a Felügyeltmappa-segéd nem fogja automatikusan feldolgozni a postaládát.
 
Az Adatmegőrzési házirendek az Exchange Felügyeleti központban:

- [Adatmegőrzési címkék és adatmegőrzési házirendek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Adatmegőrzési házirend alkalmazása postaládákra](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) vagy [Adatmegőrzési címkék hozzáadása vagy eltávolítása](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [A postaláda típusú visszatartott szöveg azonosítása](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
