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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926247"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Csoport Microsoft 365 a címlistából

Ha el Microsoft 365 az ügyfél Exchange címlistáit (például az Outlook-t vagy az OWA-t), használja az alábbi parancsot az EXO rendszerhéjban:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ha el Microsoft 365, hogy a csoport ne legyen látható Exchange ügyfél számára, használja a következő parancsot az EXO rendszerhéjban:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

