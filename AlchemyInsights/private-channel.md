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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="801ac-102">Privát csatornák a Microsoft Teamsben</span><span class="sxs-lookup"><span data-stu-id="801ac-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="801ac-103">A privát csatornák a Microsoft Teams új funkciója.</span><span class="sxs-lookup"><span data-stu-id="801ac-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="801ac-104">Ne feledje, hogy a magáncsatornák nem konvertálhatók szabványos csatornákból, és fordítva.</span><span class="sxs-lookup"><span data-stu-id="801ac-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="801ac-105">A privát csatornákkal kapcsolatos részletekért, például a [privát csatornák létrehozásáról és a tagságról,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) valamint a [privát csatorna SharePoint-webhelyekről](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)a [Privát csatornák a Microsoft Teamsben](https://docs.microsoft.com/MicrosoftTeams/private-channels)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="801ac-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="801ac-106">**Megjegyzés:** Mivel a privát csatornaüzenetek megőrzésére vonatkozó konfiguráció még nem támogatott, az adatmegőrzési házirendekkel rendelkező bérlők alapértelmezés szerint nem lesznek engedélyezve a privát csatornák.</span><span class="sxs-lookup"><span data-stu-id="801ac-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="801ac-107">A privát csatornák engedélyezhetők a Teams felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="801ac-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="801ac-108">Vegye figyelembe azt is, hogy bár a privát csatornaüzenetek megőrzése nem támogatott, a privát csatornákon megosztott fájlok megőrzése is támogatott.</span><span class="sxs-lookup"><span data-stu-id="801ac-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="801ac-109">**Új csapattulajdonosra van szüksége?**</span><span class="sxs-lookup"><span data-stu-id="801ac-109">**Need a new team owner?**</span></span>

<span data-ttu-id="801ac-110">Ha a privát csatorna tulajdonosa távozik, a Teams Powershellen keresztül új csapattulajdonost adhat hozzá.</span><span class="sxs-lookup"><span data-stu-id="801ac-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="801ac-111">A Teams Powershell telepítése [ide.](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)</span><span class="sxs-lookup"><span data-stu-id="801ac-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="801ac-112">Itt van a parancsmag lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="801ac-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="801ac-113">A Teams Powershellről a [Teams PowerShell – áttekintés című témakörben olvashat bővebben.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="801ac-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
