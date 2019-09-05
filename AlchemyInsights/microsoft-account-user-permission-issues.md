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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754194"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="b62db-102">Probléma elhárítása-a felhasználó nem található a címtárban</span><span class="sxs-lookup"><span data-stu-id="b62db-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="b62db-103">Ha a felhasználók "a felhasználó nem található" hibaüzenetet kapnak a címtárban.</span><span class="sxs-lookup"><span data-stu-id="b62db-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="b62db-104">Próbálkozzon újra, ahol a probléma típusa felhasználó nem szerepel a címtárban.</span><span class="sxs-lookup"><span data-stu-id="b62db-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="b62db-105">A probléma elhárításához hajtsa végre a következő lépéseket.</span><span class="sxs-lookup"><span data-stu-id="b62db-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="b62db-106">Ellenőrizze, hogy az e-mail meghívót elfogadó fiók ugyanaz-e, mint a későbbi bejelentkezéshez használt fiók.</span><span class="sxs-lookup"><span data-stu-id="b62db-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="b62db-107">Győződj meg a felhasználó van használ ugyanaz számla-hoz elfogad a meghív és jel levegőbe telek.</span><span class="sxs-lookup"><span data-stu-id="b62db-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="b62db-108">További információért tekintse meg, [hogyan kezelheti a Microsoft-</a> fiókjához tartozó aliasokat az Office 365 bejelentkezési adatainak](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="b62db-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="b62db-109">Tallózzon a felhasználó által a hibát fogadó hely (ek) hez.</span><span class="sxs-lookup"><span data-stu-id="b62db-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="b62db-110">Adja hozzá a "/_layouts/15/People.aspx/membershipgroupid = 0" parancsot (a dupla idézőjelek között) a webhely URL-címének végéhez.</span><span class="sxs-lookup"><span data-stu-id="b62db-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="b62db-111">Például: https://_lt_ "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="b62db-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="b62db-112">Válassza ki a felhasználót a listáról.</span><span class="sxs-lookup"><span data-stu-id="b62db-112">Select the user from the list.</span></span>

- <span data-ttu-id="b62db-113">Kattintson a **felhasználói engedélyek eltávolítása** parancsra a menüszalagon.</span><span class="sxs-lookup"><span data-stu-id="b62db-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="b62db-114">Adja vissza a felhasználót, és küldje el újra a meghívást a felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="b62db-114">Add back the User and Resend the invite to the user.</span></span>

