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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="d54f9-102">Erős jelszókövetelmény módosítása</span><span class="sxs-lookup"><span data-stu-id="d54f9-102">Change strong password requirement</span></span>

<span data-ttu-id="d54f9-103">A Microsoft alapértelmezés szerint erős jelszavakat követel meg.</span><span class="sxs-lookup"><span data-stu-id="d54f9-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="d54f9-104">A PowerShell használatával letilthatja az erős jelszavakat adott felhasználóknak az alábbi parancsokkal:</span><span class="sxs-lookup"><span data-stu-id="d54f9-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="d54f9-105">Ha minden felhasználó számára le szeretné tiltani az erős jelszavakat, használja a következőt:</span><span class="sxs-lookup"><span data-stu-id="d54f9-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="d54f9-106">További információ a jelszó-házirendről</span><span class="sxs-lookup"><span data-stu-id="d54f9-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="d54f9-107">Csatlakozás a Microsoft 365-hez a PowerShell használatával</span><span class="sxs-lookup"><span data-stu-id="d54f9-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="d54f9-108">További információ a PowerShell MsolUser parancsaival kapcsolatban</span><span class="sxs-lookup"><span data-stu-id="d54f9-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
