---
title: Az NDI-technológia bekapcsolás
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935103"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="846f0-102">Az NDI-technológia bekapcsolás</span><span class="sxs-lookup"><span data-stu-id="846f0-102">Turn on NDI technology</span></span>

<span data-ttu-id="846f0-103">Az NDI-technológia használatához két lépést kell bekapcsolni a felhasználóknak:</span><span class="sxs-lookup"><span data-stu-id="846f0-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="846f0-104">A bérlői rendszergazdának engedélyeznie kell az "AllowNDIStreaming" tulajdonságot a CsTeamsMeetingPolicy szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="846f0-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="846f0-105">Miután ez a módosítás ki lett töltve, a végfelhasználónak be kell kapcsolnia az NDI® technológiát az adott ügyfélhez a Beállítások és engedélyek **> gombra.**</span><span class="sxs-lookup"><span data-stu-id="846f0-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="846f0-106">További információt az [NDI-technológia használata a Microsoft Teamsben.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="846f0-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
