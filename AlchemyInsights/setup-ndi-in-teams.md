---
title: Az NDI-technológia bekapcsolása
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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023524"
---
# <a name="turn-on-ndi-technology"></a>Az NDI-technológia bekapcsolása

Az NDI-technológia használatához két lépést kell bekapcsolni a felhasználóknak:

1. A bérlői rendszergazdának engedélyeznie kell az "AllowNDIStreaming" tulajdonságot a CsTeamsMeetingPolicyban.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Miután ez a módosítás ki lett töltve, a felhasználónak be kell kapcsolnia az NDI®-technológiát az adott ügyfélhez a **Gépház > területen.**

További információt az [NDI-technológia használata](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)a Microsoft Teams.
