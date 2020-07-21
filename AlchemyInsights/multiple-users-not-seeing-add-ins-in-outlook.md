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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="dddbf-102">Több felhasználó nem látja a bővítményeket az Outlookban</span><span class="sxs-lookup"><span data-stu-id="dddbf-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="dddbf-103">Ha teszteli az Outlook-bővítményeket, és egyik sem jelenik meg, első hibaelhárítási lépésként a **Get-OrganizationConfig** PowerShell parancsmag segítségével kérdezze le az _AppsForOfficeEnabled_ paramétert.</span><span class="sxs-lookup"><span data-stu-id="dddbf-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="dddbf-104">Ha a lekérdezés **hamis**értéket ad vissza, állítsa ezt a paramétert **True** értékre a **Set-OrganizationConfig** parancsmag használatával, így a bővítmények a várt módon jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="dddbf-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="dddbf-105">Nem javasoljuk, hogy az _AppsForOfficeEnabled_ paraméter **értéke Hamis**.</span><span class="sxs-lookup"><span data-stu-id="dddbf-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="dddbf-106">A **Hamis** érték felülírja a fenti felügyeleti és felhasználói szerepkör-beállításokat, és megakadályozza, hogy a szervezet bármely felhasználója új alkalmazásokat aktiváljon.</span><span class="sxs-lookup"><span data-stu-id="dddbf-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="dddbf-107">További információt az [Outlook bővítményeit telepítő és kezelő rendszergazdák és felhasználók megadása](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="dddbf-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>