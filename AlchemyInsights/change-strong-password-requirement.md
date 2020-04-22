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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="ec2a0-102">Az erős jelszókövetelmény módosítása</span><span class="sxs-lookup"><span data-stu-id="ec2a0-102">Change strong password requirement</span></span>

<span data-ttu-id="ec2a0-103">A Microsoftnak alapértelmezés szerint erős jelszavakra van szüksége.</span><span class="sxs-lookup"><span data-stu-id="ec2a0-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="ec2a0-104">A PowerShell használatával ezzel a paranccsal letilthatja az erős jelszavakat bizonyos felhasználók számára:</span><span class="sxs-lookup"><span data-stu-id="ec2a0-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="ec2a0-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="ec2a0-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="ec2a0-106">További információ a jelszóházirendről</span><span class="sxs-lookup"><span data-stu-id="ec2a0-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="ec2a0-107">Csatlakozás a Microsoft 365-höz a PowerShell segítségével</span><span class="sxs-lookup"><span data-stu-id="ec2a0-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="ec2a0-108">További információ a PowerShell MsolUser parancsairól</span><span class="sxs-lookup"><span data-stu-id="ec2a0-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
