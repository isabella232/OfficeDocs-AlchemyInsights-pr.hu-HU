---
title: A SharePoint Online szabályozása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773849"
---
# <a name="sharepoint-online-throttling"></a>A SharePoint Online szabályozása

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**a 503-kiszolgáló foglalt hiba**

A felhasználók a SharePoint-vagy a OneDrive-webhelyeken való navigáláskor elfoglalt hibába ütközhet a 503-kiszolgálóval. 

Ezt a hibát a SharePoint-szolgáltatáson belüli szabályozás okozhatja. A SharePoint Online a szabályozást használja a SharePoint Online szolgáltatás optimális teljesítményének és megbízhatóságának fenntartásához. A szabályozás korlátozza a felhasználói műveletek vagy a párhuzamos hívások számát (parancsprogrammal vagy kóddal) az erőforrások túlzott felhasználásának megelőzése érdekében. 

A szabályozással kapcsolatos további tudnivalókért olvassa el a [SharePoint Online-ban a letiltott vagy Letiltva](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)jelölőnégyzetet.

Ha úgy véli, hogy ez a hiba nem kapcsolódik a szabályozáshoz, ellenőrizheti, hogy a bérlői webhelyre való navigáláskor van-e aktív [karbantartás.](https://portal.office.com/adminportal/home#/MessageCenter)

 Végül győződjön meg róla, hogy felkeresi a [szolgáltatás állapota](https://portal.office.com/adminportal/home#/servicehealth) lapot, és ellenőrizheti, hogy milyen figyelmeztetésekkel/incidensekkel fordulhat elő.

