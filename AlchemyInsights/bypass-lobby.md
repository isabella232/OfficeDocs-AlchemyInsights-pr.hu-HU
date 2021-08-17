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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059598"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Szabályozhatja az előszoba beállításait és a részvétel szintjét a Teams

Ha azt szeretné, hogy mindenki (beleértve a Betárcsázós, a Külső és a Névtelen felhasználókat is) kihagyja az előszoba kihagyásán, a PowerShell használatával elvégezheti ezt a feladatot. Az alábbi példa a szervezet globális értekezleti házirendének módosítására mutat be.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ez a parancsmag jelenleg egy PowerShell Skype Vállalati verzió modul használatát igényli. A parancsmag használatának beállítását a Házirendek kezelése [a PowerShellen keresztül](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Miután beállított egy házirendet, azt a felhasználókra kell alkalmaznia; vagy ha módosította a Globális házirendet, az automatikusan vonatkozni fog a felhasználókra. A házirendek minden módosításakor legalább 4 órát, de **legfeljebb 24** órát kell várni ahhoz, hogy a házirendek életbe lépnek. 

Mindenképpen tekintse át az alábbi dokumentációt, mielőtt ezeket a módosításokat végrehajtotta, hogy pontosan megértse, mit tesz ez lehetővé.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Az Teams előszoba házirend-vezérlőinek ismertetése

Ezekkel a beállításokkal szabályozhatja, hogy az értekezlet mely résztvevői várakozhatnak az előszoba előtt, mielőtt beengedik őket az értekezletre, és hogy milyen közreműködési szint engedélyezett az értekezleten. A PowerShell-parancsokkal frissítheti az értekezleti házirendek olyan beállításait, amelyek még nincsenek végrehajtva (a felirata "hamarosan") a Teams felügyeleti központban. Alább láthat egy PowerShell-parancsmagot, amely lehetővé teszi, hogy minden felhasználó megkerülje az előszobaet.

- [A személyek automatikus](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) beengedése szervezőnkénti házirend, amely meghatározza, hogy a felhasználók közvetlenül csatlakoznak-e egy értekezlethez, vagy az előszoba előtt várakoznak-e, amíg egy hitelesített felhasználó be nem adhatja őket.

- [A névtelen](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) személyek bekapcsolódásának engedélyezése egy szervezőnkénti házirend, amely meghatározza, hogy a névtelen személyek (beleértve a B2B-t és az összevont felhasználókat) csatlakozhatnak-e a felhasználó értekezletéhez anélkül, hogy a szervezet hitelesített felhasználója jelen van.

- [Szervezőnkénti](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) házirend, amely meghatározza, hogy a telefonon betárcsázó felhasználók közvetlenül csatlakoznak-e az értekezlethez, vagy az  előszoba előtt várakoznak-e, függetlenül attól, hogy a személyek automatikus engedjenek-e be beállítást.

- A [szervezők](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) felülbírálhatják az előszobai beállításokat **(** hamarosan) egy szervezőnkénti házirend, amely  meghatározza, hogy  az értekezlet szervezője felülbírálhatja-e az előszoba beállítását, amelyet egy rendszergazda beállított az Új értekezlet ütemezése során a betárcsázó felhasználók kihagyhatják az előszoba kihagyása című témakörben megadott beállításokat.

**Megjegyzés:** Az [értekezleti házirendek teljes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) Teams olvassa el az Értekezleti házirendek kezelése Microsoft Teams témakört.
