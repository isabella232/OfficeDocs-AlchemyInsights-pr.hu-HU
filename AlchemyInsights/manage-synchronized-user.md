---
title: Szinkronizált felhasználó kezelése
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777679"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nem lehet beállítani az elsődleges e-mail-címet, módosíthatja a felhasználói attribútumokat, vagy eltávolíthatja vagy törölheti a szinkronizált felhasználókat

Ha a címtár-szinkronizálás engedélyezve van a környezetében, akkor bizonyos felhasználói vagy objektum-attribútumok nem módosíthatók a Microsoft 365 felügyeleti központján keresztül.

A szinkronizált felhasználók és attribútumaik teljes kezeléséhez használja a helyi Active Directory-felhasználók és csoportok kezelése konzolt (adsiedit. msc).  

Azt is megteheti, hogy a szinkronizált felhasználók egyéni felhasználóit vagy attribútumait a PowerShell segítségével is megváltoztathatja, például az alábbi gyakori példákban látható módon: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
