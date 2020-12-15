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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="6b653-102">A szolgáltatott hangposta engedélyezése</span><span class="sxs-lookup"><span data-stu-id="6b653-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="6b653-103">A hangposta engedélyezéséhez a **HostedVoicemail** $True értékre kell állítani.</span><span class="sxs-lookup"><span data-stu-id="6b653-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="6b653-104">A felhasználó **HostedVoicemail** tulajdonsága távoli POWERSHELL (RPS) használatával.</span><span class="sxs-lookup"><span data-stu-id="6b653-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="6b653-105">Az RPS való csatlakozásról további információt a [Microsoft Teams PowerShell áttekintése](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="6b653-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="6b653-106">A Teams rendszergazdájának be kell jelentkeznie a Teams távoli PowerShellbe.</span><span class="sxs-lookup"><span data-stu-id="6b653-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="6b653-107">A PowerShell parancssorába a Teams rendszergazdája futtathatja a **set-csuser parancsmagnak user@contoso.com-HostedVoiceMail $truet** , ahol a SIP-URI a kérdéses felhasználó.</span><span class="sxs-lookup"><span data-stu-id="6b653-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="6b653-108">A házirendek módosításai akár 24 órát is igénybe vehetik a replikálást.</span><span class="sxs-lookup"><span data-stu-id="6b653-108">Changes to policies can take up to 24 hours to replicate.</span></span>