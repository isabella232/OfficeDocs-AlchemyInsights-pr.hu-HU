---
title: Előszoba megkerülése
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820036"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="aa1ea-102">Az előszoba beállításainak és a Teamsben való részvétel szintjének szabályozása</span><span class="sxs-lookup"><span data-stu-id="aa1ea-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="aa1ea-103">Ha azt szeretné, hogy mindenki (beleértve a Betárcsázós, a Külső és a Névtelen felhasználókat is) kihagyja az előszoba kihagyásán, a PowerShell használatával elvégezheti ezt a feladatot.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="aa1ea-104">Az alábbi példa a szervezet globális értekezleti házirendének módosítására mutat be.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="aa1ea-105">Ehhez a parancsmaghoz jelenleg a Skype Vállalati verzió PowerShell-modulját kell használni.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="aa1ea-106">A parancsmag használatának beállítását a Házirendek kezelése [a PowerShellen keresztül](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="aa1ea-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="aa1ea-107">Miután beállított egy házirendet, azt a felhasználókra kell alkalmaznia; vagy ha módosította a Globális házirendet, az automatikusan vonatkozni fog a felhasználókra.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="aa1ea-108">A házirendek minden módosításakor legalább 4 órát, de **legfeljebb 24** órát kell várni ahhoz, hogy a házirendek életbe lépnek.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="aa1ea-109">Mindenképpen tekintse át az alábbi dokumentációt, mielőtt ezeket a módosításokat végrehajtotta, hogy pontosan megértse, mit tesz ez lehetővé.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="aa1ea-110">A Teams-értekezlet előszoba házirend-vezérlőinek ismertetése</span><span class="sxs-lookup"><span data-stu-id="aa1ea-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="aa1ea-111">Ezekkel a beállításokkal szabályozhatja, hogy az értekezlet mely résztvevői várakozhatnak az előszoba előtt, mielőtt beengedik őket az értekezletre, és hogy milyen közreműködési szint engedélyezett az értekezleten.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="aa1ea-112">A PowerShell-parancsokkal frissítheti a Teams Felügyeleti központban még nem megvalósított ("hamarosan elérhető") értekezleti házirend-beállításokat.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="aa1ea-113">Alább láthat egy PowerShell-parancsmagot, amely lehetővé teszi, hogy minden felhasználó megkerülje az előszobaet.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="aa1ea-114">[A személyek automatikus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) beengedése szervezőnkénti házirend, amely meghatározza, hogy a felhasználók közvetlenül csatlakoznak-e egy értekezlethez, vagy az előszoba előtt várakoznak-e, amíg egy hitelesített felhasználó be nem adhatja őket.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="aa1ea-115">[A névtelen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) személyek bekapcsolódásának engedélyezése egy szervezőnkénti házirend, amely meghatározza, hogy a névtelen személyek (beleértve a B2B-t és az összevont felhasználókat) csatlakozhatnak-e a felhasználó értekezletéhez anélkül, hogy a szervezet hitelesített felhasználója jelen van.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="aa1ea-116">[Szervezőnkénti](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) házirend, amely meghatározza, hogy a telefonon betárcsázó felhasználók közvetlenül csatlakoznak-e az értekezlethez, vagy az  előszoba előtt várakoznak-e, függetlenül attól, hogy a személyek automatikus engedjenek-e be beállítást.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="aa1ea-117">A [szervezők](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) felülbírálhatják az előszobai beállításokat **(** hamarosan) egy szervezőnkénti házirend, amely  meghatározza, hogy  az értekezlet szervezője felülbírálhatja-e az előszoba beállítását, amelyet egy rendszergazda beállított az Új értekezlet ütemezése során a betárcsázó felhasználók kihagyhatják az előszoba kihagyása című témakörben megadott beállításokat.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="aa1ea-118">**Megjegyzés:** A [Microsoft Teams-értekezleti](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) házirendek teljes körű áttekintéséhez olvassa el az Értekezleti házirendek kezelése a Teamsben témakört.</span><span class="sxs-lookup"><span data-stu-id="aa1ea-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
