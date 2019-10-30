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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768442"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>A lobby-beállítások és a részvételi szint szabályozása

Ha azt szeretné, hogy mindenki, beleértve a betárcsázást, a külső és a névtelen felhasználók megkerüljék a lobby a Microsoft csapatok, használhatja a PowerShell segítségével csinálni. Itt egy példa a szervezet globális értekezleti házirendjének módosítására:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ez a parancsmag jelenleg a Skype for Business PowerShell modul használatát igényli. -Hoz kap beállít-hoz használ ez cmdlet, kijelenti magát [igazgató politikák keresztül PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Beállíthat egy új házirendet, amelyet ezután a felhasználókra kell alkalmaznia. Ha módosítja a globális házirendet, az automatikusan a felhasználókra is érvényes lesz. A házirendek érvénybe léptetéséhez legalább 4, illetve legfeljebb 24 órát kell várnia a házirend módosítására.

Ügyeljen arra, hogy felülvizsgálja az alábbi dokumentációt, mielőtt ezeket a változtatásokat, hogy megértsék, hogy pontosan mi ez lehetővé teszi.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>A lobby értekezleti vezérlőelemcsoportjainak ismertetése

- A [személyek automatikus beismerése](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) szervező házirend, amely azt vezérli, hogy az emberek közvetlenül csatlakoznak-e vagy várnak az előcsarnokban, amíg egy hitelesített felhasználó be nem ismerte őket.

- A [névtelen felhasználók értekezletre való indításához](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) a szervező házirend határozza meg, hogy a névtelen személyek – beleértve a B2B és az összevont felhasználókat is – csatlakozhatnak-e a felhasználó Értekezletéhez, a szervezet jelenlétében, hitelesített felhasználó nélkül.

- [Enged tárcsázz--ban használók-hoz kitérő a előszoba](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jövő nemsokára**) van egy által-szervező politika amit vezérlőberendezés Vajon emberek ki tárcsázz telefonon követ a találkozó közvetlenül vagy vár-ban előcsarnok nincs tekintettel a **gépiesen megenged emberek** elintézés.

- Az [előcsarnok beállításainak felülbírálása a szervezők számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**hamarosan**) egy szervező házirend, amely azt szabályozza, hogy az értekezlet szervezője felülírhatja-e az adott rendszergazda által beállított lobby beállításokat a **felhasználók automatikus beismerése** és a **betárcsázás engedélyezése felhasználókat, hogy megkerüljék az előcsarnokot,** amikor új találkozót ütemeznek.

**Megjegyzés:** Olvassa el az [Értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) című témakört, amely a Microsoft csapatok találkozóházirendjeinek teljes áttekintésére nyújt áttekintést.
