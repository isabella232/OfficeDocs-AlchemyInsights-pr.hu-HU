---
title: A Teams engedélyezése
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793788"
---
# <a name="enable-teams-webinars"></a>A Teams engedélyezése

A webináriumok alapértelmezés szerint engedélyezve vannak. A PowerShell-parancsokkal Teams kezelheti, hogy ki ütemezhet és regisztrálhat Teams webináriumra.

- Az értekezletek létrehozására képes összes felhasználó is létrehozhat webinárium-értekezletet. Ha szeretné kezelni, hogy ki ütemezheti a Teams, használja az *AllowMeetingRegistration lehetőséget.* 
- A *WhoCanRegister* alapértelmezés szerint engedélyezve van, és Mindenki értéket **ad meg.** Ha ki szeretné kapcsolni az értekezlet-regisztrációt, állítsa az *AllowMeetingRegistration értéket* **False (Hamis) beállításra.**

A beállítások módosításához telepítenie kell Teams [PowerShellt.](/microsoftteams/teams-powershell-install) Ezenkívül az értekezleti házirendek a webináriumok Teams is be vannak kényszerítve. Ha például az értekezlet beállításaiban kikapcsolja a névtelen csatlakozást, a névtelen felhasználók nem csatlakozhatnak webináriumhoz.

Ha többet szeretne megtudni arról, hogy ki regisztrálhat webináriumra, olvassa el A webináriumok regisztrálóira regisztrálók [konfigurálásacímet.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) A Microsoft-listák beállításairól további információt A [Microsoft-listák beállításainak szabályozása](/sharepoint/control-lists)lapon található.