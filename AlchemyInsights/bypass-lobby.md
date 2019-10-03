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
# <a name="control-lobby-settings-and-level-of-participation"></a>A lobby-beállítások és a részvételi szint szabályozása

Ezek a beállítások vezérlik, hogy a résztvevők milyen értekezletet várnak el az előtérben, mielőtt felvételt kapnak az értekezletbe, és az értekezleten részt vehetnek. A PowerShell eszközzel frissítheti a még nem végrehajtott értekezletházirend-beállításokat (a "hamarosan" felirat látható) a csapatok felügyeleti központjában.  Lásd lentebb egy példát PowerShell cmdlet, amely lehetővé teszi az összes felhasználó számára, hogy megkerülje a lobby.  

- A [személyek automatikus beismerése](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) szervező házirend, amely azt vezérli, hogy az emberek közvetlenül csatlakoznak-e vagy várnak az előcsarnokban, amíg egy hitelesített felhasználó be nem ismerte őket.

- A [névtelen felhasználók értekezletre való indításához](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) a szervező házirend határozza meg, hogy a névtelen személyek – beleértve a B2B és az összevont felhasználókat is – csatlakozhatnak-e a felhasználó Értekezletéhez, a szervezet jelenlétében, hitelesített felhasználó nélkül.

- [Enged tárcsázz--ban használók-hoz kitérő a előszoba](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jövő nemsokára**) van egy által-szervező politika amit vezérlőberendezés Vajon emberek ki tárcsázz telefonon követ a találkozó közvetlenül vagy vár-ban előcsarnok nincs tekintettel a **gépiesen megenged emberek** elintézés.

- Az [előcsarnok beállításainak felülbírálása a szervezők számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**hamarosan**) egy szervező házirend, amely azt szabályozza, hogy az értekezlet szervezője felülírhatja-e az adott rendszergazda által beállított lobby beállításokat a **felhasználók automatikus beismerése** és a **betárcsázás engedélyezése felhasználókat, hogy megkerüljék az előcsarnokot,** amikor új találkozót ütemeznek.

**Megjegyzés:** Olvassa el az [Értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) című témakört, amely a Microsoft csapatok találkozóházirendjeinek teljes áttekintésére nyújt áttekintést. 


**PowerShell példa**

Ha azt szeretné, hogy mindenki, köztük a külső vagy névtelen felhasználók is megengedjék a lobby megkerülési lehetőséget, a PowerShell segítségével is végrehajthatja ezt a feladatot.  Itt egy példa a szervezet globális értekezletházirendjének módosítására.   

(Mindenképpen nézze át a dokumentációt, mielőtt ezeket a változtatásokat megérne, hogy pontosan ezt is lehetővé teszi.)

Set-CsTeamsMeetingPolicy-identitás globális-AutoAdmittedUsers "mindenki"-AllowPSTNUsersToBypassLobby $True

További információ: [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
