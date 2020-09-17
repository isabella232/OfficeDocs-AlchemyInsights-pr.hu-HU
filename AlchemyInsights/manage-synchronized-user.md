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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="6653b-102">Nem lehet beállítani az elsődleges e-mail-címet, módosíthatja a felhasználói attribútumokat, vagy eltávolíthatja vagy törölheti a szinkronizált felhasználókat</span><span class="sxs-lookup"><span data-stu-id="6653b-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="6653b-103">Ha a címtár-szinkronizálás engedélyezve van a környezetében, akkor bizonyos felhasználói vagy objektum-attribútumok nem módosíthatók a Microsoft 365 felügyeleti központján keresztül.</span><span class="sxs-lookup"><span data-stu-id="6653b-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="6653b-104">A szinkronizált felhasználók és attribútumaik teljes kezeléséhez használja a helyi Active Directory-felhasználók és csoportok kezelése konzolt (adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="6653b-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="6653b-105">Azt is megteheti, hogy a szinkronizált felhasználók egyéni felhasználóit vagy attribútumait a PowerShell segítségével is megváltoztathatja, például az alábbi gyakori példákban látható módon:</span><span class="sxs-lookup"><span data-stu-id="6653b-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
