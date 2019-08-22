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
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506409"
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
