---
title: 902 (szinkronizálási hibák miatt az ismétlődő objektumok)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507417"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>A szinkronizálási hibák miatt az ismétlődő objektumok

Az alábbi hibaüzenetek egyike jelenhet directory szinkronizálásának befejeztével az Office 365 rendszerben:

- Nem lehet frissíteni az objektumot a Microsoft Online Services, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi könyvtárban egy másik objektumhoz társított.

- A szinkronizált objektumok proxy címe megegyezik a Microsoft Online Services könyvtárban már létezik.

- Nem lehet frissíteni az objektum, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi címtárszolgáltatás a másik objektumhoz társított: UserPrincipalName.

Azonosítására, és a probléma megoldásához töltse le és futtassa a [IdFix DirSync hiba javítására szolgáló eszköz](https://www.microsoft.com/download/details.aspx?id=36832).

További tudnivalókért lásd: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
