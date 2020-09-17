---
title: a 305 az archív postaláda méretének növelése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778585"
---
# <a name="increase-the-archive-mailbox-size"></a>Az archiválási postaláda méretének növelése


Ha azt szeretné, hogy az alábbi beállítások automatikus ellenőrzését végezze el, válassza a vissza gombot <--a lap tetején, majd adja meg annak a felhasználónak az e-mail-címét, akinek az archiválási postaláda méretére van szüksége.

A Microsoft 365 a felhasználói fiókhoz rendelt licenc alapján [korlátozza](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) az archív postaládák méretét. Amikor az archív postaláda elérte a 90%-ot, a felhasználó e-mailben értesítést kap. Ha egy archív postaláda elérte a mérethatárt, a felhasználó nem tud további elemeket áthelyezni az archív postaládába. A Microsoft 365 nem növeli meg az archív postaládák méretét, ha a mérethatárt elérte a méretet. A felhasználók az archív postaládában helyet szabadíthat fel az alábbi műveletek elvégzésével:

- Exportálja az elemeket egy. pst fájlba az Outlook használatával.

- Elemek törlése az archív postaládából.

A Microsoft 365 **korlátlan archiválási** lehetőséget biztosít az Office 365 Enterprise E3 és az E5 csomag licencekhez. A rendszergazdának engedélyeznie kell ezt a szolgáltatást, mielőtt az archív postaláda elérte a maximális méretet. Ha a korlátlan archiválás engedélyezve van, akkor akár 30 napig is eltarthat, mire a szabad terület bekerül az archív postaládába. Ezért azt javasoljuk, hogy a rendszergazdák ellenőrizzenek az archív postaláda szabad területéről, amely lehetővé teszi, hogy a felhasználó továbbra is használja az archív postaládát a kibontásban. További információt [a korlátlan archiválás áttekintése a microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) és a [korlátlan archiválás engedélyezése a Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)-on című témakörben talál.

Ha többet szeretne tudni az archív postaláda Outlookból való eléréséről, olvassa el az [Outlook követelményei az elemek automatikus kibontott archívumban való eléréséhez](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)című témakört. Ha olyan adatmegőrzési házirendet szeretne beállítani, amely automatikusan áthelyezi az elemeket az archív postaládába, olvassa el az [archiválási és törlési házirend beállítása a postaládákhoz a Microsoft 365-szervezetben](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)című cikket.

**Megjegyzés**: az automatikus bővülő archívumokat nem támogatja az elsődleges postaládák az Exchange 2010-ben.
