---
title: 902 (Szinkronizálási hibák ismétlődő objektumok miatt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767130"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Ismétlődő objektumok miatti szinkronizálási hibák

A Microsoft 365-ben a címtár-szinkronizálás befejezésekor az alábbi hibaüzenetek egyike jelenhet meg:

- Az objektum nem frissíthető a Microsoft Online Services szolgáltatásban, mert az objektumhoz társított alábbi attribútumok olyan értékekkel rendelkeznek, amelyek már társítva lehetnek a helyi címtár egy másik objektumával.

- Már létezik ugyanazzal a proxycímmel rendelkező szinkronizált objektum a Microsoft Online Services címtárban.

- Az objektum nem frissíthető, mert az objektumhoz társított következő attribútumok olyan értékekkel rendelkeznek, amelyek már társítva lehetnek a helyi címtárszolgáltatások egy másik objektumával: UserPrincipalName.

A probléma azonosításához és javításához töltse le és futtassa az [IdFix DirSync hibajavító eszközt.](https://www.microsoft.com/download/details.aspx?id=36832)

További információ: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
