---
title: Módosítás erős jelszóval kapcsolatos követelmények
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701586"
---
# <a name="change-strong-password-requirement"></a>Módosítás erős jelszóval kapcsolatos követelmények

Az erős jelszavak alapértelmezés szerint van szükség. 

PowerShell használatával letilthatja a nehezen feltörhető jelszavak ezzel a paranccsal olyan felhasználók számára:<br>
*Készlet-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [További információt a jelszóházirend](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [A PowerShell O365 csatlakozás](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [További információt a MsolUser a PowerShell-parancsok](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)