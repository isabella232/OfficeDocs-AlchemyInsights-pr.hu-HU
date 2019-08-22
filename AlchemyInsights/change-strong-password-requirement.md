---
title: Módosítás erős jelszóval kapcsolatos követelmények
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
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518761"
---
# <a name="change-strong-password-requirement"></a>Módosítás erős jelszóval kapcsolatos követelmények

Alapértelmezés szerint a Microsoft megköveteli erős jelszavakat. 

Használja a PowerShell, ezzel a paranccsal olyan felhasználók számára nehezen feltörhető jelszavak letiltása:<br>
*Készlet-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [További információt a jelszóházirend](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Hogyan szeretne kapcsolódni az Office 365 a PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [További információt a MsolUser a PowerShell-parancsok](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)