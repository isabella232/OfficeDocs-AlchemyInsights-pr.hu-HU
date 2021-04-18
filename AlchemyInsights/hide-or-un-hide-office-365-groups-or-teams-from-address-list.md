---
title: Office 365-csoportok vagy -csapatok elrejtése vagy megjelenítése a címlistából
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811458"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365-csoportok vagy -csapatok elrejtése vagy megjelenítése a címlistából

Az Exchange-ügyfelek (Outlook, OWA) címlistáiban (GAL) az alábbi EXO PowerShell-paranccsal rejtheti el vagy jelenítheti meg az Office 365-csoportokat és -csapatokat:

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Az Exchange-ügyfelekből (Outlook, OWA) az alábbi EXO PowerShell-paranccsal rejtheti el vagy jelenítheti meg az Office 365-csoportokat és -csapatokat:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Részletes útmutatóért lásd: [Office 365-csoportok elrejtése a globális címlistából és az Exchange-ügyfelekből](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
