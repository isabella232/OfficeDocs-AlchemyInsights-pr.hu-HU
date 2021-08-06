---
title: 902 (Szinkronizálási hibák duplikált objektumok miatt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998796"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Szinkronizálási hibák duplikált objektumok miatt

A címtár-szinkronizálás befejeződésével a következő hibaüzenetek egyike jelenhet Microsoft 365:

- Nem lehet frissíteni ezt az objektumot a Microsoft Online Services szolgáltatásban, mert az objektummal társított alábbi attribútumok olyan értékeket tartalmaznak, amelyek a helyi címtár egy másik objektumához is társítva lehetnek.

- Már létezik szinkronizált objektum ugyanazokkal a proxycímekkel a Microsoft Online Services címtárában.

- Nem lehet frissíteni ezt az objektumot, mert az objektumhoz tartozó alábbi attribútumok olyan értékeket tartalmaznak, amelyek már társítva vannak a helyi címtárszolgáltatások egy másik objektumával: UserPrincipalName.

A hiba azonosításához és megoldásához töltse le és futtassa az [IdFix DirSync hibajavítási eszközt.](https://github.com/Microsoft/idfix)

További információ: [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
