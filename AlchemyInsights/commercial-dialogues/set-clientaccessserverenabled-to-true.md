---
title: Set ClientAccessServerEnabled to True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320358"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Set ClientAccessServerEnabled to True

Ha nem tud megnyitni egy titkosított e-mailt, és helyette **egy rpmsg** mellékletet lát, végezze el az alábbi lépéseket:

1. Csatlakozás PowerShell Exchange Online át.

    **Megjegyzés:** Exchange Online PowerShellhez való csatlakozáshoz globális rendszergazdai vagy rendszergazdai Exchange kell bejelentkeznie.

   a. Nyissa Windows PowerShell, majd futtassa a következő parancsot:`$UserCredential = Get-Credential`
   b. A Hitelesítő **Windows PowerShell** párbeszédpanelen adja meg munkahelyi vagy iskolai fiókját és jelszavát, c. Kattintson az **OK** gombra. 

2. Futtassa az alábbi parancsot új munkamenet létrehozásához:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Futtassa az alábbi parancsot:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Futtatás `Get-IRMConfiguration` parancs.

4. Ellenőrizze **a ClientAccessServerEnabled beállítást.** 

    a. Ha **a ClientAccessServerEnabled** beállítás False (Hamis) értéket **ad** meg, futtassa az alábbi parancsmagot: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tipp:** Mindig zárja be a PowerShell-munkamenetet a következő paranccsal: `Remove-PSSession $Session`

További információt a [PowerShell Exchange Online tartalmaz.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

