---
title: A Exchange Online PowerShell használatával engedélyezheti a DKIM-et egy adott tartományhoz
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070304"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>A Exchange Online PowerShell használatával engedélyezheti a DKIM-et egy adott tartományhoz

Ha nem tudja létrehozni a DKIM DNS-rekordokat a felügyeleti központban, próbálkozzon a PowerShell Exchange Online használatával. 

A DKIM DNS-rekord PowerShell Exchange Online a következő lépésekkel hozható létre:

1. Nyissa Windows PowerShell a webhelyet rendszergazdaként, és futtassa az alábbi parancsokat a leírt sorozatban:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ha problémákat okoz a PowerShellhez való Exchange Online, a [PowerShell Csatlakozás Exchange Online tekintse át.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Miután a PowerShellhez Exchange Online, futtassa az alábbi parancsot:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Miután sikeresen végrehajtotta a fenti parancsot, futtassa az alábbi parancsot a powershell Exchange Online munkamenet megszüntetéséhez:

    `Remove-PSSession $Session` 



