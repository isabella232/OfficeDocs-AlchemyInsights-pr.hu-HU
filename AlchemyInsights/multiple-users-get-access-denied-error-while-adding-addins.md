---
title: Több felhasználó is megkapja az Access Denied hibaüzenetet, miközben bővítményeket ad hozzá az Outlook ban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423715"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Több felhasználó is megkapja az Access Denied hibaüzenetet, miközben bővítményeket ad hozzá az Outlook ban

Megadhatja, hogy a szervezet mely rendszergazdái rendelkeznek engedéllyel az Outlook bővítményeinek telepítéséhez és kezeléséhez. Azt is megadhatja, hogy a szervezet mely felhasználói jogosultak a bővítmények saját használatra történő telepítésére és kezelésére.

További információt az [Outlook bővítményeit telepítő és kezelő rendszergazdák és felhasználók megadása](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)című témakörben talál.

Annak ellenőrzéséhez, hogy sikeresen rendelt-e engedélyeket egy felhasználóhoz, cserélje le <Role Name> az ellenőrizendő szerepkör nevét, és futtassa a következő parancsot az Exchange Online PowerShellben:

Get-ManagementRoleAssignment -Role " <Role Name> " - GetEffectiveUsers

Ez a példa bemutatja, hogyan ellenőrizheti, hogy kihez rendelt engedélyeket a szervezet Office Áruházból történő telepítéséhez.

Powershell

-Szerep "Org Marketplace Apps" -GetEffectiveUsers

Az eredmények, Get-ManagementRoleAssignment tekintse át a bejegyzéseket a tényleges felhasználók oszlopban.

Részletes szintaxis- és paraméterinformációkat a [Get-ManagementRoleAssignment című](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)témakörben talál.
 