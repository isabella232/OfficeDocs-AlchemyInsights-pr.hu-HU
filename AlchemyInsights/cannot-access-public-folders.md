---
title: Nem lehet hozzáférni a nyilvános mappákhoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996632"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nyilvános mappákhoz nem lehet csatlakozni

Ha egyes felhasználók számára nem működik a nyilvános mappa elérése, próbálkozzon az alábbiakkal:

Csatlakozás EXO PowerShellt, és állítsa be a DefaultPublicFolderMailbox paramétert a problémás felhasználói fiókban úgy, hogy megfeleljen egy működő felhasználói fiók paraméterének.

Példa:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Várjon legalább egy órát, amíg a módosítás életbe lép.

Ha a probléma továbbra [](https://aka.ms/pfcte) is fennáll, az alábbi eljárással elháríthatja a nyilvános mappák elérésével kapcsolatos Outlook.
 
**Annak szabályozása, hogy mely felhasználók férnek hozzá a nyilvános mappákhoz a Outlook:**

1.  Használja Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true vagy $false  
      
    $true: Nyilvános mappák elérésének engedélyezése a felhasználóknak az Outlookban  
      
    $false: A nyilvános mappák elérésének megakadályozása az Outlookban. Ez az alapértelmezett érték.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Megjegyzés** Ez az eljárás csak az ügyfél asztali Outlook szabályozhatja Windows kapcsolatok. A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az Outlook Web App Mac Outlook.
 
További információ: A nyilvános mappákhoz való szabályozott kapcsolatok támogatása a [Outlook.](https://aka.ms/controlpf)