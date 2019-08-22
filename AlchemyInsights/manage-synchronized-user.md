---
title: Szinkronizált felhasználói kezelése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541997"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nem állítható be az elsődleges e-mail címét, vagy a felhasználói attribútumok módosítása

Ha a címtár-szinkronizálás engedélyezve van a környezetben, néhány felhasználónak vagy objektumnak attribútum nem módosítható a Microsoft 365 felügyeleti központ használatával.

Szinkronizált felhasználók és azok attribútumainak teljesen kezeléséhez használja a helyi active directory-felhasználók és csoportok kezelése konzol (adsiedit.msc).  

Azt is megteheti módosíthatja az egyes felhasználók vagy például az alábbi közös példákban látható powershell segítségével szinkronizált felhasználói attribútumok: 
- Készlet-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Készlet-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Teszt felhasználó" - Vezetéknév "Felhasználó"-"Manager" cím-osztály "HR"
- Eltávolítás-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com