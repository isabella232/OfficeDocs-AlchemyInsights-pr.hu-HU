---
title: A nyilvános mappák nem férhető hozzá
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959497"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Az Outlook nem tud kapcsolódni a nyilvános mappákhoz.

Ha a nyilvános mappához való hozzáférés néhány felhasználó esetében nem működik, próbálkozzon a következőkkel:

Csatlakozzon az EXO PowerShell környezethez, és konfigurálja a DefaultPublicFolderMailbox eszközt a problémás felhasználói fiókban úgy, hogy az megfeleljen egy működő felhasználói fióknak.

Példa:

Kap-postaláda WorkingUser | Ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Állítsa be a postafiók ProblemUser-DefaultPublicFolderMailbox \<értékét az előző parancsból>

Várjon legalább egy órát a változtatás érvénybe léptetéséhez.