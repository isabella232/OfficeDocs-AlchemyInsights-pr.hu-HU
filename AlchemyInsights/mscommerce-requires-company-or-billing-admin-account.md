---
title: Csatlakozás az MSCommerce modulhoz
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
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829738"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>Az MSCommerce használatához vállalati vagy számlázási rendszergazdai fiók szükséges

Az MSCommerce modulhoz vállalati vagy számlázási rendszergazdai jogosultsággal rendelkező fiók szükséges. Ha a következő hibaüzenet jelenik meg, újra kell csatlakoznia egy másik fiókhoz.

*ErrorMessage – A távoli kiszolgáló hibaüzenetet adott vissza: (403) Tiltott. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : Nincs megadva: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Ha a fiókja nem rendelkezik Céges vagy Számlázási rendszergazdai jogosultságokkal, forduljon a rendszergazdához.
