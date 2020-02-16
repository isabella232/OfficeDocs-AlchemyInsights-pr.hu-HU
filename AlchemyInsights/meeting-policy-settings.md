---
title: Értekezletházirend-beállításai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042846"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Értekezlet-szabályzatok kezelése a Microsoft Teamsben

**Megjegyzés: Akár 24 órát is igénybe vehet, amíg a házirend-módosítások érvénybe lépnek a felhasználók számára.** Előfordulhat, hogy nem tudja azonnal módosítani az újonnan létrehozott házirendeket; várjon 4 órát, és próbálja meg újra módosítani az újonnan létrehozott házirendet.

Az értekezlet-házirendek a szervezet felhasználói által ütemezett értekezletek résztvevői számára elérhető funkciók szabályozására szolgálnak. Előfordulhat, hogy az értekezlet-házirendek egyes funkciói még nincsenek megvalósítva a Teams felügyeleti központban (ezek a dokumentációban a "hamarosan" címkével vannak ellátva). Ebben az esetben, vagy ha olyan hibaüzenetjelenik meg, mint a "Jelenleg nem tudjuk frissíteni a szabályzatot, de próbálkozzon később" a Microsoft Teams felügyeleti központban, azt javasoljuk, hogy a PowerShell használatával hozzon létre vagy módosítsa a Teams értekezlet-szabályzatait. 

Az értekezlet-szabályzatokról az alábbi forrásokban talál további információt:

- Ha többet szeretne tudni a házirendek létrehozásáról, a módosításokról és a felhasználók házirendhez való hozzárendeléséről, olvassa el [Az értekezlet-irányelvek kezelése a Csoportokban című témakört.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Ha a PowerShell-parancsmagokkal szeretne házirend-módosításokat végrehajtani, olvassa el a [Teams PowerShell – áttekintés című témakört.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - A [Skype Vállalati verzió PowerShell-modult](https://www.microsoft.com/download/details.aspx?id=39366) kell használnia a Teams értekezlet-szabályzataihoz. 
    - További információt a [*-CsTeamsMeetingPolicy parancsmagok dokumentációjában](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) talál.

