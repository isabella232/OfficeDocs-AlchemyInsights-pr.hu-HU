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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088398"
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
