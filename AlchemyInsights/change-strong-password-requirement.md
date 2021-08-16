---
title: Erős jelszókövetelmény módosítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070686"
---
# <a name="change-strong-password-requirement"></a>Erős jelszókövetelmény módosítása

A Microsoft alapértelmezés szerint erős jelszavakat követel meg.

A PowerShell használatával letilthatja az erős jelszavakat adott felhasználóknak az alábbi parancsokkal:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Ha minden felhasználó számára le szeretné tiltani az erős jelszavakat, használja a következőt:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [További információ a jelszó-házirendről](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Csatlakozás Microsoft 365 PowerShell-parancshoz](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [További információ a PowerShell MsolUser parancsaival kapcsolatban](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
