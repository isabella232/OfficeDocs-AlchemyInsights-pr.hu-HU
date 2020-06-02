---
title: 2419-nem engedélyező-auditálás
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510430"
---
# <a name="unable-to-enable-unified-auditing"></a>Nem lehet engedélyezni az egységes naplózást

Amikor megpróbálja engedélyezni az egységes naplózást a szervezetszámára, a következőhöz hasonló hibaüzenet jelenhet meg:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

A probléma megoldásához hajtsa végre az alábbi lépéseket:

1. [Csatlakozás az Exchange Online Powershellhez](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Futtassa a következő parancsmast:

   ```
   Enable-OrganizationCustomization
   ```

3. Várjon 60 percet, amíg az előző beállítás érvénybe lép.

4. Futtassa a következő parancsot az Exchange Online PowerShellben:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

További információt az alábbi cikkekben talál:

- [Csatlakozás az Exchange Online PowerShellhez többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [A naplókeresés be- és kikapcsolása](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
