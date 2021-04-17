---
title: Értekezleti házirend beállításai
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825445"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Értekezleti házirendek kezelése a Microsoft Teamsben

**Megjegyzés: Akár 24 óra is elehet, hogy a házirendek módosításai életbe lépnek a felhasználóknál.** Előfordulhat, hogy az újonnan létrehozott házirendeket nem tudja azonnal módosításokat létrehozni; Várjon 4 órát, és próbálja meg ismét módosítani az újonnan létrehozott házirendet.

Az értekezleti házirendek a szervezet felhasználói által ütemezett értekezletek résztvevői számára elérhető funkciók szabályozását szolgálják. Előfordulhat, hogy az értekezleti házirendek egyes funkcióit még nem hajtják végre a Teams Felügyeleti központban (ezeket a dokumentációban "hamarosan" felirat jelöli). Ebben az esetben, vagy ha a Microsoft Teams Felügyeleti központban a következőhöz hasonló hibaüzenet jelenik meg: "Jelenleg nem tudjuk frissíteni a házirendet, de később újra megpróbáljuk", azt javasoljuk, hogy a PowerShell használatával hozzon létre vagy módosítson Teams-értekezleti házirendeket. 

Az értekezleti házirendekről az alábbi forrásokban talál további információt:

- Ha többet szeretne tudni a házirendek létrehozásáról, a módosításokról és a felhasználók házirendhez való hozzárendelésről, olvassa el az Értekezleti házirendek kezelése [a Teamsben részt.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- A házirendek PowerShell-parancsmagokkal való módosításairól A Teams PowerShell áttekintése [témakörben olvashat.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - A Teams-értekezleti [házirendekhez](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) a Skype Vállalati verzió PowerShell modulját kell használnia. 
    - További információt [a *-CsTeamsMeetingPolicy parancsmagok](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentációjában talál.

