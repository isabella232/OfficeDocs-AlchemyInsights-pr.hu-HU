---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007792"
---
# <a name="unable-to-enable-unified-auditing"></a>Nem lehet engedélyezni az egyesített naplózást

Amikor megpróbálja engedélyezni az egyesített naplózást a szervezetében, az alábbihoz hasonló hibaüzenet jelenhet meg:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

A probléma megoldásához kövesse az alábbi lépéseket:

1. [Csatlakozás Powershell Exchange Online át.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Futtassa az alábbi parancsmagot:

   ```
   Enable-OrganizationCustomization
   ```

3. Várjon 60 percet, amíg az előző beállítás effektusra nem lép.

4. Futtassa az alábbi parancsot Exchange Online PowerShellben:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

További információt az alábbi cikkekben talál:

- [Csatlakozás PowerShell Exchange Online többtényezős hitelesítéssel való használatának engedélyezése](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [A naplókeresés be- és kikapcsolása](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
