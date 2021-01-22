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
# <a name="turn-on-ndi-technology"></a>Az NDI-technológia bekapcsolás

Az NDI-technológia használatához két lépést kell bekapcsolni a felhasználóknak:

1. A bérlői rendszergazdának engedélyeznie kell az "AllowNDIStreaming" tulajdonságot a CsTeamsMeetingPolicy szolgáltatásban.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Miután ez a módosítás ki lett töltve, a végfelhasználónak be kell kapcsolnia az NDI® technológiát az adott ügyfélhez a Beállítások és engedélyek **> gombra.**

További információt az [NDI-technológia használata a Microsoft Teamsben.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
