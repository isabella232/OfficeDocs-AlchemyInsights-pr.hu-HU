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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055556"
---
# <a name="how-to-enable-hosted-voicemail"></a>A szolgáltatott hangposta engedélyezése

A Hangposta engedélyezéséhez **a HostedVoicemailnek** be kell állítania a $true.

The **HostedVoicemail property** on the user using Remote PowerShell (RPS).

Az RPS-hez való csatlakozásról a [PowerShell Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) témakörben olvashat bővebben az RPS-hez való csatlakozásról.

1. A Teams rendszergazdának be kell jelentkeznie a Távoli PowerShell for Teams.
1. A PowerShell parancssorában a Teams rendszergazda futtathatja a **set-user@contoso.com -HostedVoiceMail $true** parancsot, ahol a kérdéses felhasználó sip urija található.

> [!NOTE]
> A házirendek módosításainak replikálása akár 24 órát is igénybe vehet.