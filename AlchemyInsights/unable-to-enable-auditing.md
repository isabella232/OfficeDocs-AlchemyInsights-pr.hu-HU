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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="30304-102">Nem lehet engedélyezni az egyesített naplózást</span><span class="sxs-lookup"><span data-stu-id="30304-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="30304-103">Ha megkísérli engedélyezni a szervezete egyesített naplózását, az alábbihoz hasonló hibaüzenet jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="30304-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="30304-104">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="30304-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="30304-105">[Csatlakozás az Exchange Online powershellhez](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="30304-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="30304-106">Futtassa az alábbi parancsmagot:</span><span class="sxs-lookup"><span data-stu-id="30304-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="30304-107">Várjon, amíg a 60 percen belül az előző beállítás érvénybe lép.</span><span class="sxs-lookup"><span data-stu-id="30304-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="30304-108">Futtassa az alábbi parancsot az Exchange Online PowerShellben:</span><span class="sxs-lookup"><span data-stu-id="30304-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="30304-109">További információt az alábbi cikkekben talál:</span><span class="sxs-lookup"><span data-stu-id="30304-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="30304-110">Csatlakozás az Exchange Online PowerShellhez multi-Factor Authentication használatával</span><span class="sxs-lookup"><span data-stu-id="30304-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="30304-111">A naplók keresésének be-vagy kikapcsolása</span><span class="sxs-lookup"><span data-stu-id="30304-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
