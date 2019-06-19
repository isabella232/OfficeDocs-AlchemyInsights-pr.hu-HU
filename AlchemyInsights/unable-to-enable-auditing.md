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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="0391c-102">Nem lehet egységes naplózásának engedélyezése</span><span class="sxs-lookup"><span data-stu-id="0391c-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="0391c-103">Az Office 365 szervezet egységes naplózásának engedélyezése közben is megjelenhet hasonló hiba a következő:</span><span class="sxs-lookup"><span data-stu-id="0391c-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="0391c-104">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="0391c-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="0391c-105">[Az Exchange Online Powershell kapcsolódni](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="0391c-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="0391c-106">A következő parancsmag futtatásával:</span><span class="sxs-lookup"><span data-stu-id="0391c-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="0391c-107">Várja meg a korábbi beállítás érvénybe lépéséhez 60 perc.</span><span class="sxs-lookup"><span data-stu-id="0391c-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="0391c-108">Az Exchange Online PowerShell futtassa a következő parancsot:</span><span class="sxs-lookup"><span data-stu-id="0391c-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="0391c-109">További információt a következő cikkekben talál:</span><span class="sxs-lookup"><span data-stu-id="0391c-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="0391c-110">Többtényezős hitelesítést használó Exchange Online PowerShell kapcsolódni</span><span class="sxs-lookup"><span data-stu-id="0391c-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="0391c-111">Office 365 ellenőrzési napló keresés be- és kikapcsolása</span><span class="sxs-lookup"><span data-stu-id="0391c-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
