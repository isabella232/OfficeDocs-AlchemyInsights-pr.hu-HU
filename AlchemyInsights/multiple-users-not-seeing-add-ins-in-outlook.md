---
title: Több felhasználó nem látja a bővítményeket az Outlookban
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197976"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Több felhasználó nem látja a bővítményeket az Outlookban

Ha teszteli az Outlook-bővítményeket, és egyik sem jelenik meg, első hibaelhárítási lépésként a **Get-OrganizationConfig** PowerShell parancsmag segítségével kérdezze le az _AppsForOfficeEnabled_ paramétert. Ha a lekérdezés **hamis**értéket ad vissza, állítsa ezt a paramétert **True** értékre a **Set-OrganizationConfig** parancsmag használatával, így a bővítmények a várt módon jelennek meg.

Nem javasoljuk, hogy az _AppsForOfficeEnabled_ paraméter **értéke Hamis**. A **Hamis** érték felülírja a fenti felügyeleti és felhasználói szerepkör-beállításokat, és megakadályozza, hogy a szervezet bármely felhasználója új alkalmazásokat aktiváljon.

További információt az [Outlook bővítményeit telepítő és kezelő rendszergazdák és felhasználók megadása](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)című témakörben talál.