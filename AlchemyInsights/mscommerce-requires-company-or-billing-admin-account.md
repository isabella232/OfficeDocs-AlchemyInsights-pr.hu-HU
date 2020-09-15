---
title: Csatlakozás a MSCommerce modulhoz
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
- "9001212"
- "3529"
ms.openlocfilehash: 15dc7038426a8d436c236a91aa0f3462f6a3e366
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702617"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="d907c-102">A MSCommerce vállalati vagy számlázási rendszergazdai fiókot kell megadni</span><span class="sxs-lookup"><span data-stu-id="d907c-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="d907c-103">A MSCommerce modulhoz vállalati vagy számlázási rendszergazdai jogosultságokkal kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="d907c-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="d907c-104">Ha a következőhöz hasonló hibaüzenet jelenik meg, akkor újra kell majd csatlakoznia egy másik fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="d907c-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="d907c-105">*ErrorMessage – a távoli kiszolgáló hibát adott vissza: (403) tiltott. ErrorDetails – a C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 karakter: 5*</span><span class="sxs-lookup"><span data-stu-id="d907c-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="d907c-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError-ErrorContext $ _-CustomErrorMessage "nem sikerült a retri...*</span><span class="sxs-lookup"><span data-stu-id="d907c-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="d907c-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="d907c-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="d907c-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo: NotSpecified: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="d907c-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="d907c-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft. PowerShell. commands. WriteErrorException, HandleError*</span><span class="sxs-lookup"><span data-stu-id="d907c-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="d907c-110">Ha a fiókja nem rendelkezik vállalati vagy számlázási rendszergazdai jogosultságokkal, forduljon a rendszergazdához.</span><span class="sxs-lookup"><span data-stu-id="d907c-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
