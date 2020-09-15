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
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681874"
---
# <a name="change-strong-password-requirement"></a>Az erős jelszavas követelmények módosítása

A Microsoft alapértelmezés szerint erős jelszót követel meg. 

A PowerShell használatával letilthatja az erős jelszavakat az adott felhasználóknak a következő paranccsal:<br>
*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [További információ a jelszó-házirendről](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Csatlakozás a Microsoft 365-hoz a PowerShellrel](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [További információ a PowerShell MsolUser parancsairól](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
