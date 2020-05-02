---
title: Privát csatorna
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005440"
---
# <a name="private-channels-in-microsoft-teams"></a>Privát csatornák a Microsoft Teamsben

A privát csatornák a Microsoft Teams új funkciója. Ne feledje, hogy a magáncsatornák nem konvertálhatók szabványos csatornákból, és fordítva.

A privát csatornákkal kapcsolatos részletekért, például a [privát csatornák létrehozásáról és a tagságról,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) valamint a [privát csatorna SharePoint-webhelyekről](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)a [Privát csatornák a Microsoft Teamsben](https://docs.microsoft.com/MicrosoftTeams/private-channels)című témakörben talál. 

**Megjegyzés:** Mivel a privát csatornaüzenetek megőrzésére vonatkozó konfiguráció még nem támogatott, az adatmegőrzési házirendekkel rendelkező bérlők alapértelmezés szerint nem lesznek engedélyezve a privát csatornák. A privát csatornák engedélyezhetők a Teams felügyeleti központban. Vegye figyelembe azt is, hogy bár a privát csatornaüzenetek megőrzése nem támogatott, a privát csatornákon megosztott fájlok megőrzése is támogatott.

**Új csapattulajdonosra van szüksége?**

Ha a privát csatorna tulajdonosa távozik, a Teams Powershellen keresztül új csapattulajdonost adhat hozzá.


- A Teams Powershell telepítése [ide.](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)

Itt van a parancsmag lesz szüksége:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

A Teams Powershellről a [Teams PowerShell – áttekintés című témakörben olvashat bővebben.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)
