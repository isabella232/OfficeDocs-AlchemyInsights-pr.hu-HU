---
title: Az erős jelszavas követelmények módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804425"
---
# <a name="change-strong-password-requirement"></a>Az erős jelszavas követelmények módosítása

A Microsoft alapértelmezés szerint erős jelszót követel meg.

A PowerShell használatával letilthatja az erős jelszavakat az adott felhasználóknak a következő parancsokkal:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Ha az összes felhasználó erős jelszavait le szeretné tiltani, használja az alábbiakat:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [További információ a jelszó-házirendről](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Csatlakozás a Microsoft 365-hoz a PowerShellrel](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [További információ a PowerShell MsolUser parancsairól](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
