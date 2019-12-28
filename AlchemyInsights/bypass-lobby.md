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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>A lobbybeállítások és a részvétel szintje a csapatokban

Ha azt szeretné, hogy mindenki, köztük a Betárcsázás, a külső és a névtelen felhasználók is megengedjék **a lobby megkerülési**feladatát, használja a PowerShell eszközt a feladat elvégzéséhez. Itt egy példa a szervezet globális értekezletházirendjének módosítására.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ez a parancsmag jelenleg a Skype for Business PowerShell modul használatát igényli. -Hoz kap felállít-hoz használ ez cmdlet, kijelenti magát [igazgató politikák keresztül PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Miután beállította a házirendet, alkalmaznia kell azt a felhasználókra; vagy ha módosította a globális házirendet, az automatikusan a felhasználókra is érvényes lesz. A házirendek érvénybe léptetéséhez legalább **4 órát kell várni 24 óráig** , ha a házirend megváltozik. 

Ügyeljen arra, hogy felülvizsgálja az alábbi dokumentációt, mielőtt ezeket a változtatásokat, hogy megértsék, hogy pontosan mi ez lehetővé teszi.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>A lobby értekezleti vezérlőelemcsoportjainak ismertetése

Ezek a beállítások vezérlik, hogy a résztvevők milyen értekezletet várnak el az előtérben, mielőtt felvételt kapnak az értekezletbe, és az értekezleten részt vehetnek. A PowerShell eszközzel frissítheti a még nem végrehajtott értekezletházirend-beállításokat (a "hamarosan" felirat látható) a csapatok felügyeleti központjában. Lásd lentebb egy példát PowerShell cmdlet, amely lehetővé teszi az összes felhasználó számára, hogy megkerülje a lobby.

- A [személyek automatikus beismerése](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) szervező házirend, amely azt vezérli, hogy az emberek közvetlenül csatlakoznak-e vagy várnak az előcsarnokban, amíg egy hitelesített felhasználó be nem ismerte őket.

- A [névtelen felhasználók értekezletre való indításához](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) a szervező házirend határozza meg, hogy a névtelen személyek – beleértve a B2B és az összevont felhasználókat is – csatlakozhatnak-e a felhasználó Értekezletéhez, a szervezet jelenlétében, hitelesített felhasználó nélkül.

- [Enged tárcsázz--ban használók-hoz kitérő a előszoba](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jövő nemsokára**) van egy által-szervező politika amit vezérlőberendezés Vajon emberek ki tárcsázz telefonon követ a találkozó közvetlenül vagy vár-ban előcsarnok nincs tekintettel a **gépiesen megenged emberek** elintézés.

- Az előcsarnok beállításainak (**hamarosan**) [felülbírálásának engedélyezése a szervezők számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) – szervező házirend, amely azt szabályozza, hogy az értekezlet szervezője felülírhatja-e a felhasználók által **automatikusan beismerni** kívánt lobby beállításokat, és **lehetővé teszi a betárcsázó felhasználóknak, hogy az új értekezletek ütemezésekor megkerüljék az előcsarnokot** .

**Megjegyzés:** Olvassa el az [Értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) című témakört, amely a Microsoft csapatok találkozóházirendjeinek teljes áttekintésére nyújt áttekintést.
