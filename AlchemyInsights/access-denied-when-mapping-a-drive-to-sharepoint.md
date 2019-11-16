---
title: Hozzáférés megtagadva a SharePoint rendszerhez való meghajtó hozzárendelésekor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737479"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Hálózati meghajtókhoz hozzárendelt SharePoint-tárakkal kapcsolatos problémák megoldása

A csatlakoztatott hálózati meghajtók tallózásakor a következő hibaüzenetek valamelyike jelenhet meg:
  
- **\\Az elérési út nem érhető el. Lehet, hogy nincs engedélye ennek a hálózati erőforrásnak a használatára. Keresse meg a kiszolgáló rendszergazdáját, és ellenőrizze, hogy van-e hozzáférési engedélye.**

- **Hozzáférés megtagadva. Mielőtt megnyitnál fájlokat ezen a helyen, először hozzá kell adnia a webhelyet a megbízható webhelylistához, tallóznia kell a webhelyhez, és be kell jelölnie az automatikusan bejelentkező beállítást.**

[Segítség a csatlakoztatott hálózati meghajtók hibaelhárításához](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
A tárak hálózati meghajtóként való hozzárendelése csak az Internet Explorer programban lehetséges, csak átmeneti és támogatott. Ehelyett [szinkronizálja a SharePoint-fájlokat az új OneDrive szinkronizáló ügyféllel](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , amely tartalmaz [igény szerinti fájlokat](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Belépés minden-a fájlokat-ban OneDrive nélkül használ helyi raktározás hely.
  