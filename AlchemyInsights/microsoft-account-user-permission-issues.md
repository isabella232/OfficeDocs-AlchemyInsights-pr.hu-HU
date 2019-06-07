---
title: Hozzon létre, és a megosztott postafiók
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762403"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="1c22f-102">Probléma - felhasználó nem található a könyvtárban</span><span class="sxs-lookup"><span data-stu-id="1c22f-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="1c22f-103">Ha a felhasználók kapnak hiba üzenet "felhasználó nem található" a könyvtárban.</span><span class="sxs-lookup"><span data-stu-id="1c22f-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="1c22f-104">Próbálja meg újra ahol a hiba típusa nincs felhasználói könyvtárban.</span><span class="sxs-lookup"><span data-stu-id="1c22f-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="1c22f-105">Az alábbi lépéseket a probléma elhárítása hajtható végre.</span><span class="sxs-lookup"><span data-stu-id="1c22f-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="1c22f-106">Biztosítása érdekében elfogadott, az e-mail meghívóban az ugyanazt a fiókot később aláírásához használt fiók.</span><span class="sxs-lookup"><span data-stu-id="1c22f-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="1c22f-107">Győződjön meg arról, hogy a felhasználó elfogadja a meghívást, és jelentkezzen be a webhely ugyanazt a fiókot használja.</span><span class="sxs-lookup"><span data-stu-id="1c22f-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="1c22f-108">További információért lásd: [kezelése a Microsoft-fiók alias</a> kezelése az Office 365 bejelentkezési](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="1c22f-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="1c22f-109">Keresse meg minden hely, ahol a felhasználó kap a hiba.</span><span class="sxs-lookup"><span data-stu-id="1c22f-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="1c22f-110">Adjunk hozzá "/ _layouts/15/people.aspx/membershipgroupid=0" (az idézőjelek) belül a webhely URL-cím végéhez.</span><span class="sxs-lookup"><span data-stu-id="1c22f-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="1c22f-111">Példa: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="1c22f-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="1c22f-112">Jelölje ki a felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="1c22f-112">Select the user from the list.</span></span>

- <span data-ttu-id="1c22f-113">Kattintson a menüszalag **felhasználói engedélyek eltávolítása** .</span><span class="sxs-lookup"><span data-stu-id="1c22f-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="1c22f-114">Vissza a felhasználó hozzáadása, és küldje el a meghívás a felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="1c22f-114">Add back the User and Resend the invite to the user.</span></span>

