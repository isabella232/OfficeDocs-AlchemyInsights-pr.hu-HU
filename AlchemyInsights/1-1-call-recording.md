---
title: 1:1-es hívásrögzítés
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733851"
---
# <a name="11-call-recording"></a>1:1-es hívásrögzítés

A rendszergazdáknak azonnal el kell fogadnia a szükséges lépéseket ahhoz, hogy a felhasználók folytathatják az 1:1-es hívások rögzítését.
 
2021. április 12-től kezdve bevezetjük az *AllowCloudRecordingForCalls* új Teams-hívási házirend-beállítását. 

A hívásrögzítési funkciókat jelenleg a Teams-értekezleti házirendek *AllowCloudRecording* beállításával lehet vezérelni. Ha a felhasználóknak engedélyezett a Teams-értekezletek rögzítésére, az egy:1-es hívásokat is rögzíthetnek.

Ha minden felhasználót le szeretne tiltani az 1:1-es hívások rögzítésében, nem kell semmilyen műveletet megtennie. *Az AllowCloudRecordingForCalls* hívásházirend beállítása alapértelmezés szerint $False engedélyezett.

Ez a változás az Üzenetközpont következő bejegyzésében található: [(Frissítve) 1:1-es hívásrögzítési](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) házirend – Bevezetés A Teams hívási házirend beállításának beállítását a [Teams PowerShell használatával](https://docs.microsoft.com/microsoftteams/teams-powershell-install)kell beállítani.

**A hívásrögzítés engedélyezése 1:1-es hívásokban:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**A hívásrögzítés 1:1-es** hívásokban való letiltásához: Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

