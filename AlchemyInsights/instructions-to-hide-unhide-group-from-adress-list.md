---
title: A lista elrejtésének és felfedésének lépései
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663011"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>A Microsoft 365-csoport elrejtése a címlista listából (GAL)

Ha el szeretné rejteni a Microsoft 365-csoportot az Exchange-ügyfélprogramokból (például az Outlookból vagy az OWAből) származó címlistákból, használja az alábbi parancsot az EXO shellben:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ha el szeretné rejteni a Microsoft 365-csoportot az Exchange-ügyfélprogramok számára láthatóvá, használja az EXO Shell következő parancsát:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

