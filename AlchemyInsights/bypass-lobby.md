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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Az előszoba beállításainak és a Teamsben való részvétel szintjének szabályozása

Ha azt szeretné, hogy mindenki (beleértve a Betárcsázós, a Külső és a Névtelen felhasználókat is) kihagyja az előszoba kihagyásán, a PowerShell használatával elvégezheti ezt a feladatot. Az alábbi példa a szervezet globális értekezleti házirendének módosítására mutat be.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ehhez a parancsmaghoz jelenleg a Skype Vállalati verzió PowerShell-modulját kell használni. A parancsmag használatának beállítását a Házirendek kezelése [a PowerShellen keresztül](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Miután beállított egy házirendet, azt a felhasználókra kell alkalmaznia; vagy ha módosította a Globális házirendet, az automatikusan vonatkozni fog a felhasználókra. A házirendek minden módosításakor legalább 4 órát, de **legfeljebb 24** órát kell várni ahhoz, hogy a házirendek életbe lépnek. 

Mindenképpen tekintse át az alábbi dokumentációt, mielőtt ezeket a módosításokat végrehajtotta, hogy pontosan megértse, mit tesz ez lehetővé.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>A Teams-értekezlet előszoba házirend-vezérlőinek ismertetése

Ezekkel a beállításokkal szabályozhatja, hogy az értekezlet mely résztvevői várakozhatnak az előszoba előtt, mielőtt beengedik őket az értekezletre, és hogy milyen közreműködési szint engedélyezett az értekezleten. A PowerShell-parancsokkal frissítheti a Teams Felügyeleti központban még nem megvalósított ("hamarosan elérhető") értekezleti házirend-beállításokat. Alább láthat egy PowerShell-parancsmagot, amely lehetővé teszi, hogy minden felhasználó megkerülje az előszobaet.

- [A személyek automatikus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) beengedése szervezőnkénti házirend, amely meghatározza, hogy a felhasználók közvetlenül csatlakoznak-e egy értekezlethez, vagy az előszoba előtt várakoznak-e, amíg egy hitelesített felhasználó be nem adhatja őket.

- [A névtelen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) személyek bekapcsolódásának engedélyezése egy szervezőnkénti házirend, amely meghatározza, hogy a névtelen személyek (beleértve a B2B-t és az összevont felhasználókat) csatlakozhatnak-e a felhasználó értekezletéhez anélkül, hogy a szervezet hitelesített felhasználója jelen van.

- [Szervezőnkénti](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) házirend, amely meghatározza, hogy a telefonon betárcsázó felhasználók közvetlenül csatlakoznak-e az értekezlethez, vagy az  előszoba előtt várakoznak-e, függetlenül attól, hogy a személyek automatikus engedjenek-e be beállítást.

- A [szervezők](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) felülbírálhatják az előszobai beállításokat **(** hamarosan) egy szervezőnkénti házirend, amely  meghatározza, hogy  az értekezlet szervezője felülbírálhatja-e az előszoba beállítását, amelyet egy rendszergazda beállított az Új értekezlet ütemezése során a betárcsázó felhasználók kihagyhatják az előszoba kihagyása című témakörben megadott beállításokat.

**Megjegyzés:** A [Microsoft Teams-értekezleti](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) házirendek teljes körű áttekintéséhez olvassa el az Értekezleti házirendek kezelése a Teamsben témakört.
