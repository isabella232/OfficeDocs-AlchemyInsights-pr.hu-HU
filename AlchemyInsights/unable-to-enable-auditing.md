---
title: 2419 – nem engedélyezhető – naplózás
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767601"
---
# <a name="unable-to-enable-unified-auditing"></a>Nem lehet engedélyezni az egyesített naplózást

Ha megkísérli engedélyezni a szervezete egyesített naplózását, az alábbihoz hasonló hibaüzenet jelenhet meg:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

A probléma megoldásához kövesse az alábbi lépéseket:

1. [Csatlakozás az Exchange Online powershellhez](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Futtassa az alábbi parancsmagot:

   ```
   Enable-OrganizationCustomization
   ```

3. Várjon, amíg a 60 percen belül az előző beállítás érvénybe lép.

4. Futtassa az alábbi parancsot az Exchange Online PowerShellben:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

További információt az alábbi cikkekben talál:

- [Csatlakozás az Exchange Online PowerShellhez multi-Factor Authentication használatával](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [A naplók keresésének be-vagy kikapcsolása](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
