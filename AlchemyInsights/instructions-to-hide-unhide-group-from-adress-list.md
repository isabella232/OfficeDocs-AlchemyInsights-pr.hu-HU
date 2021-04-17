---
title: Instructions to hide/unhide group from address list
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831880"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Microsoft 365-csoport elrejtése a címlistából

Ha el kell rejtenie egy Microsoft 365-csoportot az Exchange-ügyfelek (például az Outlook vagy az OWA) címlistái elől, használja az alábbi parancsot az EXO rendszerhéjban:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ha el kell rejtenie a Microsoft 365-csoportot az Exchange-ügyfelek elől, használja a következő parancsot az EXO rendszerhéjban:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

