---
title: A tulajdonos nem hozhat létre almappát az Outlookkal
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836137"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>A tulajdonos nem hozhat létre almappát az Outlookkal

**Egy még folyamatban lévő hiba miatt a nyilvános mappatulajdonosok az Outlook segítségével hoznak létre almappákat. A problémát hamarosan kijavítjuk.**

Addig is használja az alábbi kerülő megoldásokat:

1. Az almappa létrehozása a MAC Outlookkal, mivel a probléma csak az asztali Outlookot (az összes verziót) érintette.
2. Az almappa exo shell vagy EAC használatával való létrehozása a rendszergazdával
3. A problémát okozó mappa DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-jának módosítása a tartalompostaládán kívül más postaládára  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Várjon egy órát, indítsa újra az Outlook ügyfélprogramot