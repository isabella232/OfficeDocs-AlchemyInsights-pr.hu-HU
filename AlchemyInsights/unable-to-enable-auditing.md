---
title: 2419-nem-a--naplózásának engedélyezése
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065653"
---
# <a name="unable-to-enable-unified-auditing"></a>Nem lehet egységes naplózásának engedélyezése

Az Office 365 szervezet egységes naplózásának engedélyezése közben is megjelenhet hasonló hiba a következő:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

A probléma megoldásához kövesse az alábbi lépéseket:

1. [Az Exchange Online Powershell kapcsolódni](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. A következő parancsmag futtatásával:

   ```
   Enable-OrganizationCustomization
   ```

3. Várja meg a korábbi beállítás érvénybe lépéséhez 60 perc.

4. Az Exchange Online PowerShell futtassa a következő parancsot:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

További információt a következő cikkekben talál:

- [Többtényezős hitelesítést használó Exchange Online PowerShell kapcsolódni](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 ellenőrzési napló keresés be- és kikapcsolása](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
