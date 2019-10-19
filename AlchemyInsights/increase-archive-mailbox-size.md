---
title: 305. az archív postaláda méretének növelése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36661802"
---
# <a name="increase-the-archive-mailbox-size"></a>Az archív postaláda méretének növelése

Hivatal 365 [határok](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) a méret-ból archív postaláda azon alapszik a engedély amit ' zárgondnok-hoz felhasználó számla. Amikor az archív postafiók eléri a megengedett 90%-ot, a felhasználó e-mail értesítést kap. Ha egy archív postaláda eléri a méretkorlátját, a felhasználó nem tud több elemet áthelyezni az archív postaládába. Hivatal 365 szokás ' növekszik a méret-ból egy archív postaláda egyszer a méret korlátoz van nyúlt. Ehelyett a következő műveletek segítségével szabadítson fel helyet az archív postaládában:

- Exportálja a. pst fájlba az Outlook segítségével.

- Elemek törlése az archív postaládából.

Hivatal 365 szolgáltat **határtalan levéltáros** részére Hivatal 365 vállalat E3 és E5 engedélyez. Egy adminisztrátornak engedélyeznie kell ezt a szolgáltatást, mielőtt az archív postaláda elérné a maximális méretet. Ha korlátlan archiválás engedélyezett, akkor akár 30 napig is eltarthat, amíg a szabad terület bekerül az archív postaládába. Ezért azt javasoljuk, hogy az adminisztrátorok ellenőrizzék a szabad területet az archív postaládában, amely lehetővé teszi, hogy a felhasználó továbbra is használja az archív postaládát a kibontásakor. További információért, lát- [Áttekintés-ból határtalan levéltáros hivatalban 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) és [képessé tesz határtalan levéltáros hivatalban 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Az archív postaláda Outlook programból való elérésével kapcsolatban további információt az [Outlook követelményei az automatikus kibontott Archívum elemeinek eléréséhez](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)című témakörben talál. Az elemeknek az archív postaládába való automatikus áthelyezéséről további adatmegőrzési szabály beállításához olvassa el az [Office 365 szervezet postafiókjainak archiválási és törlési házirendjének beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)című témakört.

**Megjegyzés**: az automatikusan bővülő archívumokat nem támogatja elsődleges postaládák az Exchange 2010-on.
