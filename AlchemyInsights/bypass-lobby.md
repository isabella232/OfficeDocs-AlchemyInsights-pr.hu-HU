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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376681"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="5efcf-102">A lobby-beállítások és a részvételi szint szabályozása</span><span class="sxs-lookup"><span data-stu-id="5efcf-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="5efcf-103">Ezek a beállítások vezérlik, hogy a résztvevők milyen értekezletet várnak el az előtérben, mielőtt felvételt kapnak az értekezletbe, és az értekezleten részt vehetnek.</span><span class="sxs-lookup"><span data-stu-id="5efcf-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="5efcf-104">A PowerShell eszközzel frissítheti a még nem végrehajtott értekezletházirend-beállításokat (a "hamarosan" felirat látható) a csapatok felügyeleti központjában.</span><span class="sxs-lookup"><span data-stu-id="5efcf-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="5efcf-105">Lásd lentebb egy példát PowerShell cmdlet, amely lehetővé teszi az összes felhasználó számára, hogy megkerülje a lobby.</span><span class="sxs-lookup"><span data-stu-id="5efcf-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="5efcf-106">A [személyek automatikus beismerése](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) szervező házirend, amely azt vezérli, hogy az emberek közvetlenül csatlakoznak-e vagy várnak az előcsarnokban, amíg egy hitelesített felhasználó be nem ismerte őket.</span><span class="sxs-lookup"><span data-stu-id="5efcf-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="5efcf-107">A [névtelen felhasználók értekezletre való indításához](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) a szervező házirend határozza meg, hogy a névtelen személyek – beleértve a B2B és az összevont felhasználókat is – csatlakozhatnak-e a felhasználó Értekezletéhez, a szervezet jelenlétében, hitelesített felhasználó nélkül.</span><span class="sxs-lookup"><span data-stu-id="5efcf-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="5efcf-108">[Enged tárcsázz--ban használók-hoz kitérő a előszoba](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jövő nemsokára**) van egy által-szervező politika amit vezérlőberendezés Vajon emberek ki tárcsázz telefonon követ a találkozó közvetlenül vagy vár-ban előcsarnok nincs tekintettel a **gépiesen megenged emberek** elintézés.</span><span class="sxs-lookup"><span data-stu-id="5efcf-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="5efcf-109">Az [előcsarnok beállításainak felülbírálása a szervezők számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**hamarosan**) egy szervező házirend, amely azt szabályozza, hogy az értekezlet szervezője felülírhatja-e az adott rendszergazda által beállított lobby beállításokat a **felhasználók automatikus beismerése** és a **betárcsázás engedélyezése felhasználókat, hogy megkerüljék az előcsarnokot,** amikor új találkozót ütemeznek.</span><span class="sxs-lookup"><span data-stu-id="5efcf-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="5efcf-110">**Megjegyzés:** Olvassa el az [Értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) című témakört, amely a Microsoft csapatok találkozóházirendjeinek teljes áttekintésére nyújt áttekintést.</span><span class="sxs-lookup"><span data-stu-id="5efcf-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="5efcf-111">**PowerShell példa**</span><span class="sxs-lookup"><span data-stu-id="5efcf-111">**PowerShell example**</span></span>

<span data-ttu-id="5efcf-112">Ha azt szeretné, hogy mindenki, köztük a külső vagy névtelen felhasználók is megengedjék a lobby megkerülési lehetőséget, a PowerShell segítségével is végrehajthatja ezt a feladatot.</span><span class="sxs-lookup"><span data-stu-id="5efcf-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="5efcf-113">Itt egy példa a szervezet globális értekezletházirendjének módosítására.</span><span class="sxs-lookup"><span data-stu-id="5efcf-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="5efcf-114">(Mindenképpen nézze át a dokumentációt, mielőtt ezeket a változtatásokat megérne, hogy pontosan ezt is lehetővé teszi.)</span><span class="sxs-lookup"><span data-stu-id="5efcf-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="5efcf-115">Set-CsTeamsMeetingPolicy-identitás globális-AutoAdmittedUsers "mindenki"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="5efcf-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="5efcf-116">További információ: [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="5efcf-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
