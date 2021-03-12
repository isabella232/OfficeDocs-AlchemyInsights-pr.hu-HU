---
title: DKIM engedélyezése adott tartományhoz az Exchange Online PowerShell használatával
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746281"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>DKIM engedélyezése adott tartományhoz az Exchange Online PowerShell használatával

Ha nem tudja létrehozni a DKIM DNS-rekordokat a felügyeleti központban, próbálkozzon az Exchange Online PowerShell használatával. 

DKIM DNS-rekord létrehozásához az Exchange Online PowerShell használatával végezze el az alábbi lépéseket:

1. Nyissa meg rendszergazdaként a Windows PowerShellt, és futtassa az alábbi parancsokat a leírt sorozatban:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ha problémákat okoz az Exchange Online PowerShellhez való csatlakozáskor, tekintse meg a Csatlakozás az [Exchange Online-hoz PowerShell használatával (lásd: Csatlakozás az Exchange Online-hoz PowerShell használatával).](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Miután csatlakozott az Exchange Online PowerShellhez, futtassa az alábbi parancsot:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Miután sikeresen végrehajtotta a fenti parancsot, futtassa az alábbi parancsot az Exchange Online PowerShell-munkamenet megszüntetéséhez:

    `Remove-PSSession $Session` 



