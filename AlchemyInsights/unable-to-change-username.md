---
title: Nem lehet módosítani a felhasználónevet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439550"
---
# <a name="unable-to-change-username"></a>Nem lehet módosítani a felhasználónevet

Bizonyos esetekben az egyszerű felhasználónév (UserPrincipalName) módosításai nem lesznek propagálva a felhőbe. Előfordulhat, hogy érvényesítési hibák at kap az Office 365 portálon, vagy nem tudja módosítani a felhasználónevet vagy az e-mail címet. A probléma megoldásához manuálisan állítsa be a UserPrincipalName parancsot ezzel a PowerShell-paranccsal.

**Példa: Felhasználó átnevezése**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Ez a parancs átnevezi davidc@contoso.com davidchew@contoso.com.

További információ: [Set-MsolUserPrincipalPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).