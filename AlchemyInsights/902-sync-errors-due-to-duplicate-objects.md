---
title: 902 (szinkronizálási hibák miatt az ismétlődő objektumok)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919874"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>A szinkronizálási hibák miatt az ismétlődő objektumok

Az alábbi hibaüzenetek egyike jelenhet directory szinkronizálásának befejeztével:
  
- Nem lehet frissíteni az objektumot a Microsoft Online Services, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi könyvtárban egy másik objektumhoz társított.
    
- A szinkronizált objektumok proxy címe megegyezik a Microsoft Online Services könyvtárban már létezik.
    
- Nem lehet frissíteni az objektum, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi címtárszolgáltatás a másik objektumhoz társított: UserPrincipalName.
    
Azonosítására, és a probléma megoldásához töltse le és futtassa a [IdFix DirSync hiba javítására szolgáló eszköz](https://www.microsoft.com/download/details.aspx?id=36832).
  
További tudnivalókért lásd: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

