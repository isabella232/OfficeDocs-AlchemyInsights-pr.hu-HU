---
title: Hozzáférés megtagadva, ha meghajtót rendel a SharePointhoz
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668745"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>A hálózati meghajtókhoz rendelt SharePoint-tárakkal kapcsolatos problémák megoldása

Egy csatlakoztatott hálózati meghajtóra való tallózáskor az alábbi üzenetek egyike jelenhet meg:
  
- **\\Az elérési út nem érhető el. Lehet, hogy nincs engedélye a hálózati erőforrás használatához. A kiszolgáló rendszergazdájától megtudhatja, hogy rendelkezik-e hozzáférési engedélyekkel.**

- **Hozzáférés megtagadva Mielőtt fájlokat nyit meg a helyen, először fel kell vennie a webhelyet a megbízható helyek listájára, tallózással keresse meg a webhelyet, és jelölje be a megfelelő Bejelentkezés automatikusan választógombot.**

[Segítséget kaphat a csatlakoztatott hálózati meghajtók hibaelhárításához](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
A tárak hálózati meghajtóként való megfeleltetése ideiglenes, és csak az Internet Explorerben támogatott. Ehelyett [szinkronizálja a SharePoint-fájlokat az új OneDrive szinkronizálási ügyfélprogrammal](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , amely az [igény szerinti fájlokat](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)tartalmazza. A OneDrive-on lévő összes fájl eléréséhez helyi tárterület használata nélkül.
  