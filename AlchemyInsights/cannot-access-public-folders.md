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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819514"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Az Outlook nem tud nyilvános mappákhoz csatlakozni

Ha egyes felhasználók számára nem működik a nyilvános mappa elérése, próbálkozzon az alábbiakkal:

Csatlakozzon az EXO PowerShellhez, és állítsa be a DefaultPublicFolderMailbox paramétert a problémás felhasználói fiókon úgy, hogy megfeleljen egy működő felhasználói fiók paraméterének.

Példa:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Várjon legalább egy órát, amíg a módosítás életbe lép.

Ha a probléma továbbra [](https://aka.ms/pfcte) is fennáll, kövesse az alábbi eljárást a nyilvános mappák elérésével kapcsolatos problémák elhárításához az Outlookkal.
 
**Annak szabályozása, hogy mely felhasználók férnek hozzá a nyilvános mappákhoz az Outlook használatával:**

1.  Használja Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true vagy $false  
      
    $true: Nyilvános mappák elérésének engedélyezése a felhasználóknak az Outlookban  
      
    $false: Felhasználói hozzáférés megakadályozása a nyilvános mappákhoz az Outlookban. Ez az alapértelmezett érték.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Megjegyzés** Ez az eljárás csak a Windows Outlook asztali verziójával létesítő kapcsolatokat szabályozhatja. A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az OWA vagy a Mac Outlook használatával.
 
További információ: [Az Outlookban](https://aka.ms/controlpf)a nyilvános mappákhoz való szabályozott kapcsolatok támogatása.