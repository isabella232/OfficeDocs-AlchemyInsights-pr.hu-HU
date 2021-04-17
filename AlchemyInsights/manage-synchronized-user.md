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
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823969"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nem lehet beállítani az elsődleges e-mail-címet, módosítani a felhasználói attribútumokat, illetve eltávolítani/törölni egy szinkronizált felhasználót

Ha engedélyezve van a címtár-szinkronizálás a környezetben, egyes felhasználói vagy objektumattribútumok nem módosíthatók a Microsoft 365 Felügyeleti központban.

A szinkronizált felhasználók és attribútumaik teljes kezeléséhez használja a helyi Active Directory-felhasználókat és csoportkezelési konzolt (adsiedit.msc).  

Másik lehetőségként a powershell használatával módosíthatja az egyes felhasználókat vagy a szinkronizált felhasználók attribútumát, például az alábbi gyakori példákban:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
