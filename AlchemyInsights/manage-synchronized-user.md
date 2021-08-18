---
title: Szinkronizált felhasználó kezelése
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114780"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nem lehet beállítani az elsődleges e-mail-címet, módosítani a felhasználói attribútumokat, illetve eltávolítani/törölni egy szinkronizált felhasználót

Ha engedélyezve van a címtár-szinkronizálás a környezetben, a felhasználói vagy objektum egyes attribútumai nem módosíthatók a Microsoft 365 Felügyeleti központ.

A szinkronizált felhasználók és attribútumaik teljes kezeléséhez használja a helyi Active Directory-felhasználókat és csoportkezelési konzolt (adsiedit.msc).  

Másik lehetőségként a powershell használatával módosíthatja az egyes felhasználókat vagy a szinkronizált felhasználók attribútumát, például az alábbi gyakori példákban:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
