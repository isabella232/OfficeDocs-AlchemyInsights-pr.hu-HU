---
title: Webinárium-regisztráció kezelése
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793918"
---
# <a name="manage-webinar-registration"></a>Webinárium-regisztráció kezelése

PowerShell-parancsokkal Teams kezelheti, hogy ki regisztrálhat Teams webináriumra. A Powershell Teams való telepítéséhez lásd: [Teams PowerShell](/microsoftteams/teams-powershell-install). 

A *WhoCanRegister* alapértelmezés szerint engedélyezve van, és a **EveryoneInCompany értéket adja meg.** Ahhoz, hogy bárki, beleértve a névtelen felhasználókat is,  regisztrálhat, az értekezleti házirendet Mindenki beállításra kell állítania a Powershell parancs használatával:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Megjegyzés:** Ha a névtelen csatlakozás ki van kapcsolva az értekezlet beállításai között, a névtelen felhasználók nem csatlakozhatnak webináriumhoz. További információért és a beállítás engedélyezéséről további információt az Értekezlet [beállításainak kezelése](/microsoftteams/meeting-settings-in-teams)a Microsoft Teams.

Ha ki szeretné kapcsolni az értekezlet-regisztrációt, állítsa az *AllowMeetingRegistration értéket* **False (Hamis) beállításra.**

Ha többet szeretne megtudni arról, hogy ki regisztrálhat webináriumra, olvassa el A webináriumok regisztrálóira regisztrálók [konfigurálásacímet.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) A Microsoft-listák beállításairól további információt A [Microsoft-listák beállításainak szabályozása](/sharepoint/control-lists)lapon található.
