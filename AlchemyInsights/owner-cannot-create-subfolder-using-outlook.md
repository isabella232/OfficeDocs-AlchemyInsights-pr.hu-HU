---
title: A tulajdonos nem tud almappát létrehozni az Outlook programmal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748909"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>A tulajdonos nem tud almappát létrehozni az Outlook programmal

**Folyamatos probléma van azzal, hogy a nyilvános mappák tulajdonosai almappákat hoznak létre az Outlook programmal. A probléma hamarosan megoldódik.**

Eközben használja az alábbi megoldások egyikét:

1. Az almappa létrehozása a MAC Outlook programmal, mivel a probléma csak az asztali Outlook ablakait érinti (az összes verzió)
2. Az almappa létrehozása az EXO Rendszerhéj vagy az EAC használatával
3. A felhasználó alapértelmezettPublicFoldermailbox/effectivePublicfoldermailbox fájljának módosítása más postaládára, mint a problémát okozó mappa Tartalompostaládája  
    - *Set-mailbox User1 alapértelmezettPublicFolderMailbox PubMBX3*
4. Várjon egy órát, indítsa újra az Outlook-ügyfelet