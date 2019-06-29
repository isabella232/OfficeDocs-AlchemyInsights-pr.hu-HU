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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380507"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nem állítható be az elsődleges e-mail címét, vagy a felhasználói attribútumok módosítása

Ha a címtár-szinkronizálás engedélyezve van a környezetnek néhány felhasználónak vagy objektumnak attribútum nem módosítható a felügyeleti központ használatával.
Szinkronizált felhasználók és azok attribútumainak teljesen kezeléséhez használja a helyi active directory-felhasználók és csoportok kezelése konzol (adsiedit.msc).  

Azt is megteheti módosíthatja az egyes felhasználók vagy például az alábbi közös példákban látható powershell segítségével szinkronizált felhasználói attribútumok: 
- Készlet-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Készlet-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Teszt felhasználó" - Vezetéknév "Felhasználó"-"Manager" cím-osztály "HR"
- Eltávolítás-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com