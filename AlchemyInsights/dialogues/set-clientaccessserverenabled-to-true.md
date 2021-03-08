---
title: A ClientAccessServerEnabled beállítása igazra
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524555"
---
# <a name="set-clientaccessserverenabled-to-true"></a>A ClientAccessServerEnabled beállítása igazra

Ha nem tud megnyitni egy titkosított e-mailt, és helyette egy **rpmsg** mellékletet lát, végezze el az alábbi lépéseket:

1. Csatlakozás az Exchange Online PowerShellhez.

> [!NOTE]
> Az Exchange Online PowerShellhez való csatlakozáshoz globális rendszergazdai vagy Exchange-rendszergazdai fiókkal kell bejelentkeznie.

   a. Nyissa meg a Windows PowerShellt, és futtassa a következő parancsot: `$UserCredential = Get-Credential`
b. A **Windows PowerShell hitelesítő** adatok kérése párbeszédpanelén adja meg munkahelyi vagy iskolai fiókját és jelszavát( c). Kattintson az **OK** gombra. 

2. Új munkamenet létrehozásához futtassa az alábbi parancsot:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Futtassa a következő parancsot:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Futtatás `Get-IRMConfiguration` parancs.

4. Ellenőrizze **a ClientAccessServerEnabled beállítást.** 

    a. Ha **a ClientAccessServerEnabled** beállítása **Hamis,** futtassa az alábbi parancsmagot: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Mindig zárja be a PowerShell-munkamenetet az alábbi paranccsal: `Remove-PSSession $Session`

További információ: [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

