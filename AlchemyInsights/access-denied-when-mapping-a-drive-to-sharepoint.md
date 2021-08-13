---
title: Access denied when mapping a drive to SharePoint
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
ms.openlocfilehash: 1ed67ec926c3e73f7a16b927729255505dfe93a0ae442a5dff9400afafb41d8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938733"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>A hálózati SharePoint megfeleltetett tárakkal kapcsolatos problémák elhárítása

Ha egy megfeleltetett hálózati meghajtóra keres rá, az alábbi üzenetek egyike látható:
  
- **\\Az elérési út nem érhető el. Előfordulhat, hogy nincs engedélye a hálózati erőforrás használatára. Lépjen kapcsolatba a kiszolgáló rendszergazdájával, és kérdezze meg, hogy rendelkezik-e hozzáférési jogosultsággal.**

- **Hozzáférés megtagadva. Mielőtt ezen a helyen nyit meg fájlokat, először fel kell vegye a webhelyet a megbízható webhelyek listájára, keresse meg a webhelyet, és válassza az automatikus bejelentkezésre lehetőséget.**

Segítség a csatlakoztatott hálózati meghajtók [hibaelhárításához.](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)
  
A tárak hálózati meghajtóként való megfeleltetése csak ideiglenes, és csak az Internet Explorerben támogatott. Ehelyett [szinkronizálja SharePoint fájlokat](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) az OneDrive szinkronizálási app ügyfélprogrammal, amely tartalmazza az [Igény szerinti fájlokat.](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx) A OneDrive-ban lévő összes fájl elérése helyi tárterület használata nélkül.
  