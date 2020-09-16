---
title: A tulajdonos nem tud almappát létrehozni az Outlookkal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665720"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>A tulajdonos nem tud almappát létrehozni az Outlookkal

**Folyamatban van egy probléma a nyilvános mappák tulajdonosainak az Outlookkal való létrehozásakor. A probléma hamarosan kijavításra kerül.**

Eközben használja az alábbi kerülő megoldások egyikét:

1. A MAC Outlook használata az almappa létrehozásához a probléma hatása csak az asztali Windows Outlook (minden verzió)
2. A rendszergazda hozza létre az almappát az EXO Shell vagy az EAC segítségével
3. A felhasználó DefaultPublicFolderMailbox/EffectivePublicFolderMailbox módosítása a problémát okozó mappa tartalmát tartalmazó postaládára  
    - *Set-Mailbox Felhasználó1 DefaultPublicFolderMailbox PubMBX3*
4. Várjon egy órát, indítsa újra az Outlook ügyfélprogramot