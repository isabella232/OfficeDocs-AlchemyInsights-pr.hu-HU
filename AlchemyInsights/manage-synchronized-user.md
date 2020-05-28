---
title: Szinkronizált felhasználó kezelése
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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407352"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nem lehet beállítani az elsődleges e-mail címet, nem lehet módosítani a felhasználói attribútumokat, illetve eltávolítani/törölni egy szinkronizált felhasználót

Ha a címtár-szinkronizálás engedélyezve van a környezetben, egyes felhasználói vagy objektumattribútumok nem módosíthatók a Microsoft 365 Felügyeleti központ használatával.

A szinkronizált felhasználók és azok összes attribútumának teljes körű kezeléséhez használja a helyi active directory-felhasználók és csoportok felügyeleti konzolját (adsiedit.msc).  

Azt is megteheti, hogy módosítja az egyes felhasználók vagy attribútumok szinkronizált felhasználók powershell használatával, például az alábbi gyakori példákban: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
