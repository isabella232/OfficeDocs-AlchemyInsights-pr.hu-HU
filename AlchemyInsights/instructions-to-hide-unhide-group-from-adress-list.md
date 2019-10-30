---
title: Utasítások-hoz eldug/megzavar csoport-ból cím oldalra dől
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768926"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Az Office 365 csoport elrejtése címlistából (GAL)

Ha el szeretne rejteni egy Office 365-csoportot az Exchange ügyfelek címlistákból (GAL) (például Outlook vagy OWA), használja a következő parancsot az EXO parancshéjban:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ha el szeretné rejteni az Office 365 csoportot az Exchange ügyfelek számára, használja az EXO rendszerhéj következő parancsát:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

