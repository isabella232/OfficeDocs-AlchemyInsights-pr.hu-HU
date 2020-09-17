---
title: Nem érhetők el a nyilvános mappák
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812549"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Az Outlook nem tud csatlakozni nyilvános mappákhoz

Ha a nyilvános mappákhoz való hozzáférés néhány felhasználónál nem működött, próbálkozzon az alábbiakkal:

Csatlakozzon az EXO PowerShellhez, és állítsa be a DefaultPublicFolderMailbox paramétert a problémás felhasználói fiókban, hogy megegyezzenek a megfelelő felhasználói fiók paraméterével.

Például

Get-Mailbox WorkingUser | Ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Várjon legalább egy órát, amíg a módosítás érvénybe lép.

Ha a probléma továbbra is fennáll, kérjük, kövesse az alábbi [lépéseket](https://aka.ms/pfcte) a nyilvános mappák elérésével kapcsolatos hibák elhárítása az Outlookkal.
 
**Annak szabályozása, hogy mely felhasználók érhetik el nyilvános mappákat az Outlookkal**:

1.  Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE vagy $FALSE  
      
    $true: hozzáférés engedélyezése a felhasználóknak nyilvános mappákhoz az Outlookban  
      
    $false: felhasználók hozzáférésének megakadályozása az Outlookban elérhető nyilvános mappákhoz. Ez az alapértelmezett érték.  
        
2.  Set-OrganizationalSetting-PublicFolderShowClientControl $true   
      
**Note (Megjegyzés** ) Ez az eljárás csak a Windows Outlook asztali verziókkal használható a kapcsolat vezérlésére. A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az OWA vagy a Mac Outlook használatával.
 
További információt az [ellenőrzött kapcsolatok támogatása a nyilvános mappákhoz az Outlookban](https://aka.ms/controlpf)című témakörben talál.