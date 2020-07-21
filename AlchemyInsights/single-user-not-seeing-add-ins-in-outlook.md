---
title: Az egyfelhasználós bővítmények nem látnak az Outlookban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197961"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Az egyfelhasználós bővítmények nem látnak az Outlookban

Előfordulhat, hogy a felhasználó egy olyan szerepkör része, amely nem rendelkezik a megfelelő AppsForOfficeEnabled paraméterrel. Futtassa ezt a parancsmaskát, és derítse ki, hogy a megfelelő szerepkör van-e társítva a felhasználóhoz:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegálás $false | Format-Table -Automatikus szerepkör,RoleAssigneeName,RoleAssigneeType

További információt az [Outlook bővítményeit telepítő és kezelő rendszergazdák és felhasználók megadása](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)című témakörben talál.
