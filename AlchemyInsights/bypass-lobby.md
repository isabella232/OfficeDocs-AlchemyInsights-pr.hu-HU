---
title: Lobby mellőzése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684952"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="23c76-102">A lobby beállításainak és a részvételi szint vezérlése a Teams-ban</span><span class="sxs-lookup"><span data-stu-id="23c76-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="23c76-103">Ha mindenki számára engedélyezni szeretné a betárcsázós, a külső és a névtelen felhasználókat, hogy **kihagyja az előszobát**, használja a PowerShellt a feladat elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="23c76-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="23c76-104">Íme egy példa a szervezet globális értekezlet-házirendjének módosítására.</span><span class="sxs-lookup"><span data-stu-id="23c76-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="23c76-105">Ez a parancsmag jelenleg a Skype vállalati verzió PowerShell-modul használatát igényli.</span><span class="sxs-lookup"><span data-stu-id="23c76-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="23c76-106">Ha be szeretné állítani a parancsmag használatát, tanulmányozza a [házirendek kezelése a PowerShell segítségével](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)című cikkben talál segítséget.</span><span class="sxs-lookup"><span data-stu-id="23c76-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="23c76-107">Ha beállított egy házirendet, azt a felhasználókra kell alkalmaznia; Ha módosította a globális házirendet, akkor az automatikusan a felhasználókra lesz érvényes.</span><span class="sxs-lookup"><span data-stu-id="23c76-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="23c76-108">Bármely házirend-módosítás esetén legalább **4 órát** kell várnia, amíg a házirendek hatályba lépnek.</span><span class="sxs-lookup"><span data-stu-id="23c76-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="23c76-109">Ügyeljen arra, hogy nézze át az alábbi dokumentációt, mielőtt a módosítások pontosan megértsék, hogy mi ez a funkció.</span><span class="sxs-lookup"><span data-stu-id="23c76-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="23c76-110">A Teams-értekezlet lobbijának házirend-vezérlőinek ismertetése</span><span class="sxs-lookup"><span data-stu-id="23c76-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="23c76-111">Ezekkel a beállításokkal szabályozhatja, hogy az értekezlet résztvevői milyen mértékben várjon az előszobába, mielőtt beengedik őket az értekezletbe, és milyen mértékben vehetnek részt az értekezleten.</span><span class="sxs-lookup"><span data-stu-id="23c76-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="23c76-112">A PowerShell segítségével frissítheti az értekezlet-összehívásokat, amelyeket még nem hajtottak végre ("hamarosan") a Teams felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="23c76-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="23c76-113">Lásd alább egy példa PowerShell-parancsmagot, amely lehetővé teszi, hogy minden felhasználó kihagyja az előszobát.</span><span class="sxs-lookup"><span data-stu-id="23c76-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="23c76-114">A szervezők [automatikusan bevallják](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , hogy az értekezletek automatikusan bekapcsolódnak az értekezletbe, vagy az előszobában maradnak, amíg egy hitelesített felhasználó beengedi őket.</span><span class="sxs-lookup"><span data-stu-id="23c76-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="23c76-115">Az [értekezletek indításának engedélyezése a névtelen személyek számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) : a szervezői házirend, amely szabályozza, hogy a névtelen személyek – például a vállalatközi és az összevont felhasználók – csatlakozhatnak-e a felhasználó Értekezletéhez anélkül, hogy a szervezeten belüli részvételt engedélyeztek.</span><span class="sxs-lookup"><span data-stu-id="23c76-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="23c76-116">[A betárcsázós felhasználók kihagyhatják az előszobát](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**hamarosan**elérhető) a szervezői házirend, amely azt szabályozza, hogy a telefonos hívással betárcsázó személyek közvetlenül vagy várjon az előszobában, függetlenül attól, hogy a **személyek automatikusan bevallják** -e ezt a beállítást.</span><span class="sxs-lookup"><span data-stu-id="23c76-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="23c76-117">A [szervezők számára lehetővé teszi a lobby-beállítások felülbírálását](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**hamarosan**) a szervezői házirend, amely azt szabályozza, hogy az értekezlet szervezője felülbírálja-e az előszoba beállításait, amelyeket a rendszergazda **automatikusan Bevallhat** , és **engedélyezheti a betárcsázós felhasználóknak, hogy az** új értekezletek ütemezésekor megkerüljék az előszobát.</span><span class="sxs-lookup"><span data-stu-id="23c76-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="23c76-118">**Megjegyzés:** Olvassa el a [Teams értekezlet-házirendek kezelése a Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) alkalmazásban a Microsoft Teams-értekezleti házirendek teljes áttekintését.</span><span class="sxs-lookup"><span data-stu-id="23c76-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
