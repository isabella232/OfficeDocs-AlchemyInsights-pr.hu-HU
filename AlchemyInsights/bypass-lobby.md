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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889084"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="5e3e3-102">A lobbybeállítások és a részvétel szintje a csapatokban</span><span class="sxs-lookup"><span data-stu-id="5e3e3-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="5e3e3-103">Ha azt szeretné, hogy mindenki, köztük a Betárcsázás, a külső és a névtelen felhasználók is megengedjék **a lobby megkerülési**feladatát, használja a PowerShell eszközt a feladat elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="5e3e3-104">Itt egy példa a szervezet globális értekezletházirendjének módosítására.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="5e3e3-105">Ez a parancsmag jelenleg a Skype for Business PowerShell modul használatát igényli.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="5e3e3-106">-Hoz kap felállít-hoz használ ez cmdlet, kijelenti magát [igazgató politikák keresztül PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="5e3e3-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="5e3e3-107">Miután beállította a házirendet, alkalmaznia kell azt a felhasználókra; vagy ha módosította a globális házirendet, az automatikusan a felhasználókra is érvényes lesz.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="5e3e3-108">A házirendek érvénybe léptetéséhez legalább **4 órát kell várni 24 óráig** , ha a házirend megváltozik.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="5e3e3-109">Ügyeljen arra, hogy felülvizsgálja az alábbi dokumentációt, mielőtt ezeket a változtatásokat, hogy megértsék, hogy pontosan mi ez lehetővé teszi.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="5e3e3-110">A lobby értekezleti vezérlőelemcsoportjainak ismertetése</span><span class="sxs-lookup"><span data-stu-id="5e3e3-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="5e3e3-111">Ezek a beállítások vezérlik, hogy a résztvevők milyen értekezletet várnak el az előtérben, mielőtt felvételt kapnak az értekezletbe, és az értekezleten részt vehetnek.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="5e3e3-112">A PowerShell eszközzel frissítheti a még nem végrehajtott értekezletházirend-beállításokat (a "hamarosan" felirat látható) a csapatok felügyeleti központjában.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="5e3e3-113">Lásd lentebb egy példát PowerShell cmdlet, amely lehetővé teszi az összes felhasználó számára, hogy megkerülje a lobby.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="5e3e3-114">A [személyek automatikus beismerése](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) szervező házirend, amely azt vezérli, hogy az emberek közvetlenül csatlakoznak-e vagy várnak az előcsarnokban, amíg egy hitelesített felhasználó be nem ismerte őket.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="5e3e3-115">A [névtelen felhasználók értekezletre való indításához](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) a szervező házirend határozza meg, hogy a névtelen személyek – beleértve a B2B és az összevont felhasználókat is – csatlakozhatnak-e a felhasználó Értekezletéhez, a szervezet jelenlétében, hitelesített felhasználó nélkül.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="5e3e3-116">[Enged tárcsázz--ban használók-hoz kitérő a előszoba](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jövő nemsokára**) van egy által-szervező politika amit vezérlőberendezés Vajon emberek ki tárcsázz telefonon követ a találkozó közvetlenül vagy vár-ban előcsarnok nincs tekintettel a **gépiesen megenged emberek** elintézés.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="5e3e3-117">Az előcsarnok beállításainak (**hamarosan**) [felülbírálásának engedélyezése a szervezők számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) – szervező házirend, amely azt szabályozza, hogy az értekezlet szervezője felülírhatja-e a felhasználók által **automatikusan beismerni** kívánt lobby beállításokat, és **lehetővé teszi a betárcsázó felhasználóknak, hogy az új értekezletek ütemezésekor megkerüljék az előcsarnokot** .</span><span class="sxs-lookup"><span data-stu-id="5e3e3-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="5e3e3-118">**Megjegyzés:** Olvassa el az [Értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) című témakört, amely a Microsoft csapatok találkozóházirendjeinek teljes áttekintésére nyújt áttekintést.</span><span class="sxs-lookup"><span data-stu-id="5e3e3-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
