---
title: A szolgáltatott hangposta engedélyezése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318650"
---
# <a name="how-to-enable-hosted-voicemail"></a>A szolgáltatott hangposta engedélyezése

A Hangposta engedélyezéséhez **a HostedVoicemailnek** be kell állítania a $true.

The **HostedVoicemail property** on the user using Remote PowerShell (RPS).

Az RPS-hez való csatlakozásról a [PowerShell Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) témakörben olvashat bővebben az RPS-hez való csatlakozásról.

1. A Teams rendszergazdának be kell jelentkeznie a távoli PowerShell-Teams.
1. A PowerShell parancssorában a Teams rendszergazda futtathatja a **set-user@contoso.com -HostedVoiceMail $true,** ahol a kérdéses felhasználó sip urija található.

**Megjegyzés:** A házirendek módosításainak replikálása akár 24 órát is igénybe vehet.