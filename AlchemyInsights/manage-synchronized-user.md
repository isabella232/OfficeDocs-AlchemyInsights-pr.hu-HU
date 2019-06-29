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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="ff3d7-102">Nem állítható be az elsődleges e-mail címét, vagy a felhasználói attribútumok módosítása</span><span class="sxs-lookup"><span data-stu-id="ff3d7-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="ff3d7-103">Ha a címtár-szinkronizálás engedélyezve van a környezetnek néhány felhasználónak vagy objektumnak attribútum nem módosítható a felügyeleti központ használatával.</span><span class="sxs-lookup"><span data-stu-id="ff3d7-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="ff3d7-104">Szinkronizált felhasználók és azok attribútumainak teljesen kezeléséhez használja a helyi active directory-felhasználók és csoportok kezelése konzol (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="ff3d7-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="ff3d7-105">Azt is megteheti módosíthatja az egyes felhasználók vagy például az alábbi közös példákban látható powershell segítségével szinkronizált felhasználói attribútumok:</span><span class="sxs-lookup"><span data-stu-id="ff3d7-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="ff3d7-106">Készlet-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ff3d7-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="ff3d7-107">Készlet-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Teszt felhasználó" - Vezetéknév "Felhasználó"-"Manager" cím-osztály "HR"</span><span class="sxs-lookup"><span data-stu-id="ff3d7-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="ff3d7-108">Eltávolítás-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ff3d7-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>