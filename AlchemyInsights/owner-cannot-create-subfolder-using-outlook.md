---
title: A tulajdonos nem hozhat létre almappát a Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063126"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>A tulajdonos nem hozhat létre almappát a Outlook

**Egy még folyamatban lévő probléma miatt a nyilvános mappatulajdonosok almappákat hoznak létre az Outlook. A problémát hamarosan kijavítjuk.**

Addig is használja az alábbi kerülő megoldásokat:

1. Az almappa Outlook MAC rendszeren használható, mivel a probléma csak az asztali Outlook (az összes verzióban)
2. Az almappa exo shell vagy EAC használatával való létrehozása a rendszergazdával
3. A problémát okozó mappa DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-jának módosítása a tartalompostaládán kívül más postaládára  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Várjon egy órát, indítsa újra az Outlook ügyfélprogramot