---
title: Értekezlet-házirend beállításai
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794336"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Értekezlet-házirendek kezelése a Microsoft Teams alkalmazásban

**Megjegyzés: akár 24 óra is eltelhet, amíg a házirend módosítása a felhasználók számára érvényben lesz.** Előfordulhat, hogy nem tudja azonnal módosítani az újonnan létrehozott házirendeket; várjon 4 órát, és próbálja meg ismét módosítani az újonnan létrehozott házirendet.

Az értekezlet-házirendek a szervezet felhasználói által ütemezett értekezletekhez a résztvevők számára elérhető funkciók szabályozására szolgálnak. Az értekezlet-összehívások bizonyos funkciói nem hajthatók végre a Teams felügyeleti központban, (ezeket a "hamarosan elérhető" felirat jelzi a dokumentációban). Ebben az esetben, vagy ha hibaüzenetet kap, például "nem tudjuk frissíteni a házirendet, de később újra próbálkozni", a Microsoft Teams felügyeleti központjában azt javasoljuk, hogy a PowerShell segítségével hozza létre vagy módosítsa a Teams-értekezletekre vonatkozó házirendeket. 

Az értekezlet-házirendekről további információt az alábbi forrásokban talál:

- Ha tudni szeretné, hogy miként hozhat létre házirendeket, és hogyan módosíthatja a felhasználókat a házirendhez, olvassa el az [értekezlet-házirendek kezelése a Teams alkalmazásban](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)című témakört.

- Ha PowerShell-parancsmagokkal szeretné módosítani a házirendet, olvassa el a [Teams PowerShell áttekintése](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)című témakört. 
    - A Teams Meeting-házirendjeihez a [Skype vállalati verzió PowerShell-modult](https://www.microsoft.com/download/details.aspx?id=39366) kell használnia. 
    - További információért tekintse át a [*-CsTeamsMeetingPolicy parancsmagok dokumentációját](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

