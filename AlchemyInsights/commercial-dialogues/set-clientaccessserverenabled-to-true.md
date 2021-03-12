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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746414"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Set ClientAccessServerEnabled to True

Ha nem tud megnyitni egy titkosított e-mailt, és helyette **egy rpmsg** mellékletet lát, végezze el az alábbi lépéseket:

1. Csatlakozás az Exchange Online PowerShellhez.

> [!NOTE]
> Az Exchange Online PowerShellhez való csatlakozáshoz globális rendszergazdai vagy Exchange-rendszergazdai fiókkal kell bejelentkeznie.

   a. Nyissa meg a Windows PowerShellt, és futtassa a következő parancsot: `$UserCredential = Get-Credential`
b. A **Windows PowerShell** hitelesítő adatok kérése párbeszédpanelen adja meg munkahelyi vagy iskolai fiókját és jelszavát, c. Kattintson az **OK** gombra. 

2. Futtassa az alábbi parancsot új munkamenet létrehozásához:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Futtassa a következő parancsot:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Futtatás `Get-IRMConfiguration` parancs.

4. Ellenőrizze **a ClientAccessServerEnabled beállítást.** 

    a. Ha **a ClientAccessServerEnabled** beállítás **False (Hamis)** értéket ad meg, futtassa az alábbi parancsmagot: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Mindig zárja be a PowerShell-munkamenetet a következő paranccsal: `Remove-PSSession $Session`

További információ: [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

