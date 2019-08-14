---
title: 305 archív postaláda méretének növelése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 28086145d8769bd06ef6352257a820146c5f237d
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391329"
---
# <a name="increase-the-archive-mailbox-size"></a>Az archív postaláda méretének növelése

Office 365 [határértékek](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) alapján a licencet a felhasználói fiókhoz rendelt archív postaládák méretét. Az archív postaláda mérete megengedett mérete 90 %-át, amikor a felhasználó kap e-mailben értesítjük. Az archív postaláda eléri a maximális méretét, ha a felhasználó nem további elemek áthelyezése az archív postaláda. Az Office 365 nem az archív postaláda méretének növelése, amint elérik a maximális méretét. Ehelyett a felhasználók az archív postaládában helyet szabadíthat fel a következő műveletek hajthatók végre:

- Exportálja a az elemeket egy .pst fájl az Outlook programmal

- Elemek törlése az archív postaláda.

Office 365 biztosít **korlátlan archiválási** Office 365 vállalati E3, E5 és licencek. Egy rendszergazda engedélyezni kell a szolgáltatást, mielőtt az archív postaláda eléri a maximális méretét. Ha korlátlan archiválási engedélyezve van, legfeljebb 30 nappal megelőzően szabad lemezterület hozzáadódik az archív postaláda is eltarthat. Emiatt javasoljuk, hogy a rendszergazdák ellenőrizze a szabad lemezterület a postafiók archívum, amely lehetővé teszi a felhasználó továbbra is használni az archív postaláda, miközben bővíti. További információt talál [az Office 365 rendszerben korlátlan archiválási áttekintése](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) és [az Office 365 rendszerben korlátlan archiválásának engedélyezése](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)

Az Outlook programból az archív postaláda elérésével kapcsolatban további információt lásd: [Outlook követelmények eléréséhez szükséges elemek automatikus bővített archívumot](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Adja meg egy adatmegőrzési szabályt, amely automatikusan átmozgatja a cikkeket az archív postaládába, olvassa el [az Office 365 szervezetben postafiókok archív és törlés házirend beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Megjegyzés**: meghagyni archívumok elsődleges postafiókok Exchange 2010 nem támogatja.
