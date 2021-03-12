---
title: Értekezleti házirend beállításai
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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704608"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Értekezleti házirendek kezelése a Microsoft Teamsben

**Megjegyzés: Akár 24 óra is elehet, hogy a házirend módosításai életbe lépnek a felhasználóknál.** Előfordulhat, hogy nem lehet azonnal módosításokat létrehozni az újonnan létrehozott házirendeket; várjon 4 órát, és próbálja meg ismét módosítani az újonnan létrehozott házirendet.

Az értekezleti házirendek a szervezet felhasználói által ütemezett értekezletek résztvevői számára elérhető funkciók szabályozását szolgálják. Előfordulhat, hogy az értekezleti házirendek egyes funkcióit még nem hajtják végre a Teams Felügyeleti központban (ezeket a dokumentációban "hamarosan" felirattal jelölték). Ebben az esetben, vagy ha a Microsoft Teams Felügyeleti központban a következőhöz hasonló hibaüzenet jelenik meg: "Jelenleg nem tudjuk frissíteni a házirendet, de később újra megpróbáljuk", azt javasoljuk, hogy a PowerShell használatával hozzon létre vagy módosítson Teams-értekezleti házirendeket. 

Az értekezleti házirendekkel kapcsolatos további információkért lásd az alábbi forrásokat:

- Ha többet szeretne tudni a házirendek létrehozásáról, a módosításokról és a felhasználók házirendhez való hozzárendelésről, olvassa el az Értekezleti házirendek kezelése [a Teamsben.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- A házirendEk PowerShell-parancsmagokkal való módosításairól a Teams PowerShell áttekintése [nyújt áttekintést.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - A Skype Vállalati [verzió PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) modulját kell használnia a Teams-értekezleti házirendek esetén. 
    - További információt [a *-CsTeamsMeetingPolicy parancsmagok dokumentációjában](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) talál.

