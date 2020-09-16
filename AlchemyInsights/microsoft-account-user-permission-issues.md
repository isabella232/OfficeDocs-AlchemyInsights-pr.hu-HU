---
title: Probléma elhárítása – a felhasználó nem található a címtárban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725409"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="3efa1-102">Probléma elhárítása – a felhasználó nem található a címtárban</span><span class="sxs-lookup"><span data-stu-id="3efa1-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="3efa1-103">Ha a felhasználó "a felhasználó nem található" hibaüzenet jelenik meg a címtárban, próbálkozzon újra, ha a probléma típusa nem a címtárban van a felhasználó.</span><span class="sxs-lookup"><span data-stu-id="3efa1-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="3efa1-104">A probléma megoldásához az alábbi lépéseket kell végrehajtania.</span><span class="sxs-lookup"><span data-stu-id="3efa1-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="3efa1-105">Gondoskodjon arról, hogy az e-mail-meghívót fogadó fiók ugyanazt a fiókot használja, amelyet később kell bejelentkezne.</span><span class="sxs-lookup"><span data-stu-id="3efa1-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="3efa1-106">Győződjön meg arról, hogy a felhasználó ugyanazt a fiókot használja a meghívás elfogadásához és a webhelyre való bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="3efa1-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="3efa1-107">További információt a Microsoft- [fiókhoz tartozó aliasok kezelése a microsoft </a> 365-beli bejelentkezés kezeléséhez](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="3efa1-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="3efa1-108">Tallózással keresse meg azokat a webhelyeket, amelyekben a felhasználó a hibát kapja.</span><span class="sxs-lookup"><span data-stu-id="3efa1-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="3efa1-109">"/_Layouts/15/People.aspx/membershipgroupid = 0" (a dupla idézőjelek között) a webhely URL-címének végére.</span><span class="sxs-lookup"><span data-stu-id="3efa1-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="3efa1-110">Példa: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="3efa1-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="3efa1-111">Jelölje ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="3efa1-111">Select the user from the list.</span></span>

- <span data-ttu-id="3efa1-112">Kattintson a **felhasználó engedélyeinek eltávolítása** elemre a menüszalagon.</span><span class="sxs-lookup"><span data-stu-id="3efa1-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="3efa1-113">Adja hozzá a felhasználót, és küldje el újra a meghívót a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="3efa1-113">Add back the User and Resend the invite to the user.</span></span>

