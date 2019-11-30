---
title: Az előcsarnok figyelmen kívül hagyása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626350"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="f72dd-102">A lobby-beállítások és a részvételi szint szabályozása</span><span class="sxs-lookup"><span data-stu-id="f72dd-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="f72dd-103">Ha azt szeretné, hogy mindenki, beleértve a betárcsázást, a külső és a névtelen felhasználók megkerüljék a lobby a Microsoft csapatok, használhatja a PowerShell segítségével csinálni.</span><span class="sxs-lookup"><span data-stu-id="f72dd-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="f72dd-104">Itt egy példa a szervezet globális értekezleti házirendjének módosítására:</span><span class="sxs-lookup"><span data-stu-id="f72dd-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="f72dd-105">Ez a parancsmag jelenleg a Skype for Business PowerShell modul használatát igényli.</span><span class="sxs-lookup"><span data-stu-id="f72dd-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="f72dd-106">-Hoz kap beállít-hoz használ ez cmdlet, kijelenti magát [igazgató politikák keresztül PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="f72dd-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="f72dd-107">Beállíthat egy új házirendet, amelyet ezután a felhasználókra kell alkalmaznia.</span><span class="sxs-lookup"><span data-stu-id="f72dd-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="f72dd-108">Ha módosítja a globális házirendet, az automatikusan a felhasználókra is érvényes lesz.</span><span class="sxs-lookup"><span data-stu-id="f72dd-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="f72dd-109">A házirendek érvénybe léptetéséhez legalább 4, illetve legfeljebb 24 órát kell várnia a házirend módosítására.</span><span class="sxs-lookup"><span data-stu-id="f72dd-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="f72dd-110">Ügyeljen arra, hogy felülvizsgálja az alábbi dokumentációt, mielőtt ezeket a változtatásokat, hogy megértsék, hogy pontosan mi ez lehetővé teszi.</span><span class="sxs-lookup"><span data-stu-id="f72dd-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="f72dd-111">A lobby értekezleti vezérlőelemcsoportjainak ismertetése</span><span class="sxs-lookup"><span data-stu-id="f72dd-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="f72dd-112">A [személyek automatikus beismerése](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) szervező házirend, amely azt vezérli, hogy az emberek közvetlenül csatlakoznak-e vagy várnak az előcsarnokban, amíg egy hitelesített felhasználó be nem ismerte őket.</span><span class="sxs-lookup"><span data-stu-id="f72dd-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="f72dd-113">A [névtelen felhasználók értekezletre való indításához](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) a szervező házirend határozza meg, hogy a névtelen személyek – beleértve a B2B és az összevont felhasználókat is – csatlakozhatnak-e a felhasználó Értekezletéhez, a szervezet jelenlétében, hitelesített felhasználó nélkül.</span><span class="sxs-lookup"><span data-stu-id="f72dd-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="f72dd-114">[Enged tárcsázz--ban használók-hoz kitérő a előszoba](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jövő nemsokára**) van egy által-szervező politika amit vezérlőberendezés Vajon emberek ki tárcsázz telefonon követ a találkozó közvetlenül vagy vár-ban előcsarnok nincs tekintettel a **gépiesen megenged emberek** elintézés.</span><span class="sxs-lookup"><span data-stu-id="f72dd-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="f72dd-115">Az előcsarnok beállításainak (**hamarosan**) [felülbírálásának engedélyezése a szervezők számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) – szervező házirend, amely azt szabályozza, hogy az értekezlet szervezője felülírhatja-e a felhasználók által **automatikusan beismerni** kívánt lobby beállításokat, és **lehetővé teszi a betárcsázó felhasználóknak, hogy az új értekezletek ütemezésekor megkerüljék az előcsarnokot** .</span><span class="sxs-lookup"><span data-stu-id="f72dd-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="f72dd-116">**Megjegyzés:** Olvassa el az [Értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) című témakört, amely a Microsoft csapatok találkozóházirendjeinek teljes áttekintésére nyújt áttekintést.</span><span class="sxs-lookup"><span data-stu-id="f72dd-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
