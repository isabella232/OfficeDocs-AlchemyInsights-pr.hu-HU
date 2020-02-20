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
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>Az MSCommerce vállalati vagy számlázási rendszergazdai fiókot igényel

Az MSCommerce modulhoz vállalati vagy számlázási rendszergazdai jogosultságokkal rendelkező fiók szükséges. Ha a következő hibaüzenet jelenik meg, újra kapcsolatba kell lépnie egy másik fiókkal.

*ErrorMessage - A távoli kiszolgáló hibát adott vissza: (403) Tiltott. Hibarészletek – A C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Nem sikerült visszaretri ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Írási hiba], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Teljesen minősítetthibaazonosító : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Ha fiókja nem rendelkezik vállalati vagy számlázási rendszergazdai jogosultságokkal, forduljon a rendszergazdához.
