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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994867"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Set ClientAccessServerEnabled to True

Ha nem tud megnyitni egy titkosított e-mailt, és helyette **egy rpmsg** mellékletet lát, végezze el az alábbi lépéseket:

1. Csatlakozás PowerShell Exchange Online át.

> [!NOTE]
> Ha a PowerShell Exchange Online szeretne csatlakozni, globális rendszergazdai vagy rendszergazdai Exchange kell bejelentkeznie.

   a. Nyissa Windows PowerShell, majd futtassa a következő parancsot:`$UserCredential = Get-Credential`
b. A Hitelesítő **Windows PowerShell** párbeszédpanelen adja meg munkahelyi vagy iskolai fiókját és jelszavát, c. Kattintson az **OK** gombra. 

2. Futtassa az alábbi parancsot új munkamenet létrehozásához:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Futtassa az alábbi parancsot:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Futtatás `Get-IRMConfiguration` parancs.

4. Ellenőrizze **a ClientAccessServerEnabled beállítást.** 

    a. Ha **a ClientAccessServerEnabled** beállítás **False (Hamis)** értéket ad meg, futtassa az alábbi parancsmagot: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Mindig zárja be a PowerShell-munkamenetet a következő paranccsal: `Remove-PSSession $Session`

További információt a [PowerShell Exchange Online tartalmaz.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

