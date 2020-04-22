---
title: Az erős jelszókövetelmény módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706563"
---
# <a name="change-strong-password-requirement"></a>Az erős jelszókövetelmény módosítása

A Microsoftnak alapértelmezés szerint erős jelszavakra van szüksége. 

A PowerShell használatával ezzel a paranccsal letilthatja az erős jelszavakat bizonyos felhasználók számára:<br>
*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*

- [További információ a jelszóházirendről](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Csatlakozás a Microsoft 365-höz a PowerShell segítségével](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [További információ a PowerShell MsolUser parancsairól](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
