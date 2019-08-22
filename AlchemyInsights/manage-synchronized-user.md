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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="f587f-102">Nem állítható be az elsődleges e-mail címét, vagy a felhasználói attribútumok módosítása</span><span class="sxs-lookup"><span data-stu-id="f587f-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="f587f-103">Ha a címtár-szinkronizálás engedélyezve van a környezetben, néhány felhasználónak vagy objektumnak attribútum nem módosítható a Microsoft 365 felügyeleti központ használatával.</span><span class="sxs-lookup"><span data-stu-id="f587f-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="f587f-104">Szinkronizált felhasználók és azok attribútumainak teljesen kezeléséhez használja a helyi active directory-felhasználók és csoportok kezelése konzol (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="f587f-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="f587f-105">Azt is megteheti módosíthatja az egyes felhasználók vagy például az alábbi közös példákban látható powershell segítségével szinkronizált felhasználói attribútumok:</span><span class="sxs-lookup"><span data-stu-id="f587f-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="f587f-106">Készlet-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f587f-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="f587f-107">Készlet-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Teszt felhasználó" - Vezetéknév "Felhasználó"-"Manager" cím-osztály "HR"</span><span class="sxs-lookup"><span data-stu-id="f587f-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="f587f-108">Eltávolítás-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f587f-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>