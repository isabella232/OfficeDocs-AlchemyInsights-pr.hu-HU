---
title: Probléma elhárítása-a felhasználó nem található a címtárban
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768803"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="cf570-102">Probléma elhárítása-a felhasználó nem található a címtárban</span><span class="sxs-lookup"><span data-stu-id="cf570-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="cf570-103">Ha használók van kap hiba üzenet "felhasználó vidám ' lenni alapít"-ban címtár, legyen szíves megpróbál újra hol a kérdés típus van felhasználó nem-ban címtár.</span><span class="sxs-lookup"><span data-stu-id="cf570-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="cf570-104">A probléma elhárításához hajtsa végre a következő lépéseket.</span><span class="sxs-lookup"><span data-stu-id="cf570-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="cf570-105">Ellenőrizze, hogy az e-mail meghívót elfogadó fiók ugyanaz-e, mint a későbbi bejelentkezéshez használt fiók.</span><span class="sxs-lookup"><span data-stu-id="cf570-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="cf570-106">Győződj meg a felhasználó van használ ugyanaz számla-hoz elfogad a meghív és jel levegőbe telek.</span><span class="sxs-lookup"><span data-stu-id="cf570-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="cf570-107">További információért tekintse meg, [hogyan kezelheti a Microsoft-</a> fiókjához tartozó aliasokat az Office 365 bejelentkezési adatainak](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="cf570-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="cf570-108">Tallózzon a felhasználó által a hibát fogadó hely (ek) hez.</span><span class="sxs-lookup"><span data-stu-id="cf570-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="cf570-109">Adja hozzá a "/_layouts/15/People.aspx/membershipgroupid = 0" parancsot (a dupla idézőjelek között) a webhely URL-címének végéhez.</span><span class="sxs-lookup"><span data-stu-id="cf570-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="cf570-110">Példa: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="cf570-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="cf570-111">Válassza ki a felhasználót a listáról.</span><span class="sxs-lookup"><span data-stu-id="cf570-111">Select the user from the list.</span></span>

- <span data-ttu-id="cf570-112">Kattintson a **felhasználói engedélyek eltávolítása** parancsra a menüszalagon.</span><span class="sxs-lookup"><span data-stu-id="cf570-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="cf570-113">Adja vissza a felhasználót, és küldje el újra a meghívást a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="cf570-113">Add back the User and Resend the invite to the user.</span></span>

