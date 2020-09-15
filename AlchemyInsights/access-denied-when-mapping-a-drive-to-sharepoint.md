---
title: Hozzáférés megtagadva, ha meghajtót rendel a SharePointhoz
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668745"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="8beb6-102">A hálózati meghajtókhoz rendelt SharePoint-tárakkal kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="8beb6-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="8beb6-103">Egy csatlakoztatott hálózati meghajtóra való tallózáskor az alábbi üzenetek egyike jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="8beb6-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="8beb6-104">**\\Az elérési út nem érhető el. Lehet, hogy nincs engedélye a hálózati erőforrás használatához. A kiszolgáló rendszergazdájától megtudhatja, hogy rendelkezik-e hozzáférési engedélyekkel.**</span><span class="sxs-lookup"><span data-stu-id="8beb6-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="8beb6-105">**Hozzáférés megtagadva Mielőtt fájlokat nyit meg a helyen, először fel kell vennie a webhelyet a megbízható helyek listájára, tallózással keresse meg a webhelyet, és jelölje be a megfelelő Bejelentkezés automatikusan választógombot.**</span><span class="sxs-lookup"><span data-stu-id="8beb6-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="8beb6-106">[Segítséget kaphat a csatlakoztatott hálózati meghajtók hibaelhárításához](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="8beb6-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="8beb6-107">A tárak hálózati meghajtóként való megfeleltetése ideiglenes, és csak az Internet Explorerben támogatott.</span><span class="sxs-lookup"><span data-stu-id="8beb6-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="8beb6-108">Ehelyett [szinkronizálja a SharePoint-fájlokat az új OneDrive szinkronizálási ügyfélprogrammal](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , amely az [igény szerinti fájlokat](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="8beb6-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="8beb6-109">A OneDrive-on lévő összes fájl eléréséhez helyi tárterület használata nélkül.</span><span class="sxs-lookup"><span data-stu-id="8beb6-109">Access all your files in OneDrive without using local storage space.</span></span>
  