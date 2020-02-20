---
title: Csatlakozás az MSCommerce modulhoz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 10ef2e8fa7c564d53177a52136eb48cd709e5c55
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158507"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="2ed04-102">Az MSCommerce vállalati vagy számlázási rendszergazdai fiókot igényel</span><span class="sxs-lookup"><span data-stu-id="2ed04-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="2ed04-103">Az MSCommerce modulhoz vállalati vagy számlázási rendszergazdai jogosultságokkal rendelkező fiók szükséges.</span><span class="sxs-lookup"><span data-stu-id="2ed04-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="2ed04-104">Ha a következő hibaüzenet jelenik meg, újra kapcsolatba kell lépnie egy másik fiókkal.</span><span class="sxs-lookup"><span data-stu-id="2ed04-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="2ed04-105">*ErrorMessage - A távoli kiszolgáló hibát adott vissza: (403) Tiltott. Hibarészletek – A C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="2ed04-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="2ed04-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Nem sikerült visszaretri ...*</span><span class="sxs-lookup"><span data-stu-id="2ed04-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="2ed04-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="2ed04-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="2ed04-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Írási hiba], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="2ed04-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="2ed04-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Teljesen minősítetthibaazonosító : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="2ed04-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="2ed04-110">Ha fiókja nem rendelkezik vállalati vagy számlázási rendszergazdai jogosultságokkal, forduljon a rendszergazdához.</span><span class="sxs-lookup"><span data-stu-id="2ed04-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
