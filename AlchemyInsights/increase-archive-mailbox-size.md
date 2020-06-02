---
title: 305 Az archív postaláda méretének növelése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f80b2a10ebc17cd98ed1d29b0e6ba3ca01eb1d62
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508810"
---
# <a name="increase-the-archive-mailbox-size"></a>Az archív postaláda méretének növelése

A Microsoft [365](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) korlátozza az archív postaládák méretét a felhasználói fiókhoz rendelt licenc alapján. Amikor az archív postaláda eléri az engedélyezett méret 90%-át, a felhasználó e-mailértesítést kap. Amikor egy archív postaláda eléri a méretkorlátot, a felhasználó nem tud több elemet áthelyezni az archív postaládába. A Microsoft 365 nem növeli az archív postaláda méretét a méretkorlát elérése után. Ehelyett a felhasználók a következő műveletekkel szabadíthatnak fel helyet az archív postaládában:

- Exportálja az elemeket .pst fájlba az Outlook programmal.

- Elemek törlése az archív postaládából.

A Microsoft 365 **korlátlan archiválást** biztosít az Office 365 Nagyvállalati E3 és E5 licenceihez. A rendszergazdának engedélyeznie kell ezt a funkciót, mielőtt az archív postaláda eléri a maximális méretét. Ha a korlátlan archiválás engedélyezve van, akár 30 napig is eltarthat, amíg a szabad terület hozzáadódik az archív postaládához. Ezért azt javasoljuk, hogy a rendszergazdák ellenőrizzék a szabad helyet az archív postafiókban, amely lehetővé teszi a felhasználó számára, hogy továbbra is használja az archív postaládát, miközben kibontja. További információt a [Korlátlan archiválás áttekintése a Microsoft 365-ben](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) és [a Korlátlan archiválás engedélyezése a Microsoft 365-ben](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)című témakörben talál.

Az archív postaláda Outlookból való eléréséről az [Outlook automatikusan kibővített archívumában lévő elemek elérésére vonatkozó követelményei](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)című témakörben talál további információt. Ha olyan adatmegőrzési szabályt szeretne beállítani, amely automatikusan áthelyezi az elemeket az archív postaládába, olvassa el Az [archiválási és törlési házirend beállítása a Microsoft 365-szervezet postaládáihoz című témakört.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**Megjegyzés:** Az Exchange 2010-en az elsődleges postaládák nem támogatják az automatikusan bővített archívumokat.
