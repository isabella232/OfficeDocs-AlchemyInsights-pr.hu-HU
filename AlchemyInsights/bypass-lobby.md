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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>A lobby beállításainak és a részvételi szint vezérlése a Teams-ban

Ha mindenki számára engedélyezni szeretné a betárcsázós, a külső és a névtelen felhasználókat, hogy **kihagyja az előszobát**, használja a PowerShellt a feladat elvégzéséhez. Íme egy példa a szervezet globális értekezlet-házirendjének módosítására.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ez a parancsmag jelenleg a Skype vállalati verzió PowerShell-modul használatát igényli. Ha be szeretné állítani a parancsmag használatát, tanulmányozza a [házirendek kezelése a PowerShell segítségével](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)című cikkben talál segítséget.

Ha beállított egy házirendet, azt a felhasználókra kell alkalmaznia; Ha módosította a globális házirendet, akkor az automatikusan a felhasználókra lesz érvényes. Bármely házirend-módosítás esetén legalább **4 órát** kell várnia, amíg a házirendek hatályba lépnek. 

Ügyeljen arra, hogy nézze át az alábbi dokumentációt, mielőtt a módosítások pontosan megértsék, hogy mi ez a funkció.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>A Teams-értekezlet lobbijának házirend-vezérlőinek ismertetése

Ezekkel a beállításokkal szabályozhatja, hogy az értekezlet résztvevői milyen mértékben várjon az előszobába, mielőtt beengedik őket az értekezletbe, és milyen mértékben vehetnek részt az értekezleten. A PowerShell segítségével frissítheti az értekezlet-összehívásokat, amelyeket még nem hajtottak végre ("hamarosan") a Teams felügyeleti központban. Lásd alább egy példa PowerShell-parancsmagot, amely lehetővé teszi, hogy minden felhasználó kihagyja az előszobát.

- A szervezők [automatikusan bevallják](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , hogy az értekezletek automatikusan bekapcsolódnak az értekezletbe, vagy az előszobában maradnak, amíg egy hitelesített felhasználó beengedi őket.

- Az [értekezletek indításának engedélyezése a névtelen személyek számára](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) : a szervezői házirend, amely szabályozza, hogy a névtelen személyek – például a vállalatközi és az összevont felhasználók – csatlakozhatnak-e a felhasználó Értekezletéhez anélkül, hogy a szervezeten belüli részvételt engedélyeztek.

- [A betárcsázós felhasználók kihagyhatják az előszobát](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**hamarosan**elérhető) a szervezői házirend, amely azt szabályozza, hogy a telefonos hívással betárcsázó személyek közvetlenül vagy várjon az előszobában, függetlenül attól, hogy a **személyek automatikusan bevallják** -e ezt a beállítást.

- A [szervezők számára lehetővé teszi a lobby-beállítások felülbírálását](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**hamarosan**) a szervezői házirend, amely azt szabályozza, hogy az értekezlet szervezője felülbírálja-e az előszoba beállításait, amelyeket a rendszergazda **automatikusan Bevallhat** , és **engedélyezheti a betárcsázós felhasználóknak, hogy az** új értekezletek ütemezésekor megkerüljék az előszobát.

**Megjegyzés:** Olvassa el a [Teams értekezlet-házirendek kezelése a Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) alkalmazásban a Microsoft Teams-értekezleti házirendek teljes áttekintését.
