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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677999"
---
# <a name="how-to-enable-hosted-voicemail"></a>A szolgáltatott hangposta engedélyezése

A hangposta engedélyezéséhez a **HostedVoicemail** $True értékre kell állítani.

A felhasználó **HostedVoicemail** tulajdonsága távoli POWERSHELL (RPS) használatával.

Az RPS való csatlakozásról további információt a [Microsoft Teams PowerShell áttekintése](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) című témakörben talál.

1. A Teams rendszergazdájának be kell jelentkeznie a Teams távoli PowerShellbe.
1. A PowerShell parancssorába a Teams rendszergazdája futtathatja a **set-csuser parancsmagnak user@contoso.com-HostedVoiceMail $truet** , ahol a SIP-URI a kérdéses felhasználó.

> [!NOTE]
> A házirendek módosításai akár 24 órát is igénybe vehetik a replikálást.