---
title: A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699521"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál

1. A Microsoft 365 felügyeleti központban nyissa meg a tartomány **beállítása**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) lapot, és a tartományok listájában válassza ki a webhelyhez használni kívánt tartományt.

2. Válassza az **+ Új egyéni rekord** elemet, és írja be az alábbiakat:

  - A **DNS típusa** mezőbe írja be az **A (Address)** értéket.

  - Az **Állomásnév vagy alias** mezőbe írja be a **@** karaktert.

  - Az **IP-cím** mezőbe írja be a statikus IP-címet, ahol a webhelye jelenleg üzemel (például 172.16.140.1).

    Ennek a webhely  *statikus*  , és nem  *dinamikus*  IP-címének kell lennie. Azt a helyet ellenőrizve, ahol a webhelye üzemel, győződjön meg arról, hogy beszerezhet statikus IP-címet a nyilvános webhelyéhez.

3. Válassza a **Mentés** elemet.

Ezenkívül egy CNAME rekordot is létrehozhat, hogy az ügyfelek könnyebben megtalálják a webhelyet.
  
1. Válassza az **+ Új egyéni rekord** elemet, és írja be az alábbiakat:

  - A **DNS típusa** mezőbe írja be a **CNAME (Alias)** értéket.

  - Az **Állomásnév vagy alias** mezőbe írja be a **www** értéket.

  - A **Célcím** mezőbe írja be a webhely teljes tartománynevét (FQDN) (például: contoso.com).

2. Válassza a **Mentés** lehetőséget.
