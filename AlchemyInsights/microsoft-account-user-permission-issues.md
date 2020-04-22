---
title: Hibaelhárítás – A felhasználó nem található a címtárban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702740"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="0c70b-102">Hibaelhárítás – A felhasználó nem található a címtárban</span><span class="sxs-lookup"><span data-stu-id="0c70b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="0c70b-103">Ha a felhasználók a "felhasználó nem található" hibaüzenetet kapják a címtárban, próbálkozzon újra ott, ahol a probléma típusa nem a címtárban található.</span><span class="sxs-lookup"><span data-stu-id="0c70b-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="0c70b-104">A probléma elhárításához a következő lépések hajthatók végre.</span><span class="sxs-lookup"><span data-stu-id="0c70b-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="0c70b-105">Győződjön meg arról, hogy az e-mail meghívót elfogadó fiók ugyanaz a fiók, amelyet a későbbi bejelentkezéshez használnak.</span><span class="sxs-lookup"><span data-stu-id="0c70b-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="0c70b-106">Győződjön meg arról, hogy a felhasználó ugyanazt a fiókot használja a meghívás elfogadásához és a webhelyre való bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="0c70b-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="0c70b-107">További információ: [A</a> Microsoft 365-ös bejelentkezés isztanevek kezelése.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="0c70b-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="0c70b-108">Tallózással keresse meg azokat a webhelyeket, amelyekben a felhasználó megkapja a hibát.</span><span class="sxs-lookup"><span data-stu-id="0c70b-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="0c70b-109">Adja hozzá a "/_layouts/15/people.aspx/membershipgroupid=0"-t (a dupla idézőjelek között) a webhely URL-címének végéhez.</span><span class="sxs-lookup"><span data-stu-id="0c70b-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="0c70b-110">Példa: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="0c70b-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="0c70b-111">Válassza ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="0c70b-111">Select the user from the list.</span></span>

- <span data-ttu-id="0c70b-112">Kattintson **a Felhasználói engedélyek eltávolítása** a menüszalagról elemre.</span><span class="sxs-lookup"><span data-stu-id="0c70b-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="0c70b-113">Adja hozzá a felhasználót, és küldje el újra a meghívót a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="0c70b-113">Add back the User and Resend the invite to the user.</span></span>

