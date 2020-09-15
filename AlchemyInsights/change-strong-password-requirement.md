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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="d29d3-102">Az erős jelszavas követelmények módosítása</span><span class="sxs-lookup"><span data-stu-id="d29d3-102">Change strong password requirement</span></span>

<span data-ttu-id="d29d3-103">A Microsoft alapértelmezés szerint erős jelszót követel meg.</span><span class="sxs-lookup"><span data-stu-id="d29d3-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="d29d3-104">A PowerShell használatával letilthatja az erős jelszavakat az adott felhasználóknak a következő paranccsal:</span><span class="sxs-lookup"><span data-stu-id="d29d3-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="d29d3-105">*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="d29d3-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="d29d3-106">További információ a jelszó-házirendről</span><span class="sxs-lookup"><span data-stu-id="d29d3-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="d29d3-107">Csatlakozás a Microsoft 365-hoz a PowerShellrel</span><span class="sxs-lookup"><span data-stu-id="d29d3-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="d29d3-108">További információ a PowerShell MsolUser parancsairól</span><span class="sxs-lookup"><span data-stu-id="d29d3-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
