---
title: 902 (szinkronizálási hibák az ismétlődő objektumok miatt)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737343"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Duplikált objektumokból adódó szinkronizálási hibák

Az alábbi hibaüzenetek egyike jelenhet meg, ha a címtár-szinkronizálás befejeződött a Microsoft 365:

- Nem lehet frissíteni az objektumot a Microsoft Online Services szolgáltatásban, mert az objektumhoz társított alábbi attribútumok olyan értékek, amelyek már társítva vannak egy másik objektummal a helyi címtárban.

- A Microsoft Online Services címtárban már létezik egy olyan szinkronizált objektum, amely ugyanazzal a proxy-címmel rendelkezik.

- Nem lehet frissíteni az objektumot, mert az objektumhoz társított alábbi attribútumok olyan értékek, amelyek már társítva vannak egy másik objektummal a helyi címtárszolgáltatásban: UserPrincipalName.

A probléma felismeréséhez és kijavításához töltse le és futtassa az IdFix-ös- [adatszervizelési hiba](https://www.microsoft.com/download/details.aspx?id=36832)

További információt a [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)című témakörben talál.
