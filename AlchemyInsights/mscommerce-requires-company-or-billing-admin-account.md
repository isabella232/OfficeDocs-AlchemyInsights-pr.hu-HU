---
title: Csatlakozás MSCommerce modulba
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
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974671"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>Az MSCommerce használatához vállalati vagy számlázási rendszergazdai fiók szükséges

Az MSCommerce modulhoz vállalati vagy számlázási rendszergazdai jogosultsággal rendelkező fiók szükséges. Ha a következő hibaüzenet jelenik meg, újra kell csatlakoznia egy másik fiókhoz.

*ErrorMessage – A távoli kiszolgáló hibaüzenetet adott vissza: (403) Tiltott. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : Nincs megadva: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Ha a fiókja nem rendelkezik Céges vagy Számlázási rendszergazdai jogosultságokkal, forduljon a rendszergazdához.
