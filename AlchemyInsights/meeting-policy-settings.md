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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925167"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Értekezleti házirendek kezelése a Microsoft Teams

**Megjegyzés: Akár 24 óra is elehet, hogy a házirendek módosításai életbe lépnek a felhasználóknál.** Előfordulhat, hogy az újonnan létrehozott házirendeket nem tudja azonnal módosításokat létrehozni; Várjon 4 órát, és próbálja meg ismét módosítani az újonnan létrehozott házirendet.

Az értekezleti házirendek a szervezet felhasználói által ütemezett értekezletek résztvevői számára elérhető funkciók szabályozását szolgálják. Előfordulhat, hogy az értekezleti házirendek egyes funkcióit még nem hajtják végre Teams Felügyeleti központban (ezeket a dokumentációban a "Hamarosan" felirat jelöli). Ebben az esetben, vagy ha a Microsoft Teams Felügyeleti központban a következőhöz hasonló hibaüzenet jelenik meg: "Jelenleg nem tudjuk frissíteni a házirendet, de később újra megpróbáljuk", azt javasoljuk, hogy a Power Teams Shell használatával hozzon létre vagy módosítson értekezleti házirendeket. 

Az értekezleti házirendekről az alábbi forrásokban talál további információt:

- A házirendek létrehozásáról, a módosításokról és a felhasználók házirendhez való hozzárendelését az Értekezleti házirendek kezelése a következő [Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- A házirendek PowerShell-parancsmagokkal való módosításairól A [PowerShell Teams témakörben olvashat.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Az értekezleti házirendek Skype Vállalati verzió [PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) modult kell Teams használnia. 
    - További információt [a *-CsTeamsMeetingPolicy parancsmagok](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentációjában talál.

