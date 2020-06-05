---
title: Utasítások a csoport elrejtésére/felfedésére a címlistából
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580011"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>A Microsoft 365-csoport elrejtése a címlistából (GAL)

Ha el szeretne rejteni egy Microsoft 365-ös csoportot az Exchange-ügyfelek (például az Outlook vagy az OWA) címlistáiból, használja a következő parancsot az EXO rendszerhéjban:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ha el szeretné rejteni, hogy a Microsoft 365 csoport nem lesz látható az Exchange-ügyfelek számára, használja a következő parancsot az EXO rendszerhéjban:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

