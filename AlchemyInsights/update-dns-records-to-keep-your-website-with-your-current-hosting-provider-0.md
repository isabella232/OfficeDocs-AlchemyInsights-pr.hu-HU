---
title: A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925287"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál

1. A [tartományok](https://portal.office.com/adminportal/home#/Domains) lapon a tartományok listában jelölje ki a tartományt, a webhely használata.

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
