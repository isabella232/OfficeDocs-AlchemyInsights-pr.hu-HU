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
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818470"
---
# <a name="change-strong-password-requirement"></a>Erős jelszókövetelmény módosítása

A Microsoft alapértelmezés szerint erős jelszavakat követel meg.

A PowerShell használatával letilthatja az erős jelszavakat adott felhasználóknak az alábbi parancsokkal:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Ha minden felhasználó számára le szeretné tiltani az erős jelszavakat, használja a következőt:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [További információ a jelszó-házirendről](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Csatlakozás a Microsoft 365-hez a PowerShell használatával](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [További információ a PowerShell MsolUser parancsaival kapcsolatban](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
