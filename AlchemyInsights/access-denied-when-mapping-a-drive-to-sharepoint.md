---
title: Hozzáférés megtagadva a SharePoint rendszerhez való meghajtó hozzárendelésekor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737479"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="66f0c-102">Hálózati meghajtókhoz hozzárendelt SharePoint-tárakkal kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="66f0c-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="66f0c-103">A csatlakoztatott hálózati meghajtók tallózásakor a következő hibaüzenetek valamelyike jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="66f0c-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="66f0c-104">**\\Az elérési út nem érhető el. Lehet, hogy nincs engedélye ennek a hálózati erőforrásnak a használatára. Keresse meg a kiszolgáló rendszergazdáját, és ellenőrizze, hogy van-e hozzáférési engedélye.**</span><span class="sxs-lookup"><span data-stu-id="66f0c-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="66f0c-105">**Hozzáférés megtagadva. Mielőtt megnyitnál fájlokat ezen a helyen, először hozzá kell adnia a webhelyet a megbízható webhelylistához, tallóznia kell a webhelyhez, és be kell jelölnie az automatikusan bejelentkező beállítást.**</span><span class="sxs-lookup"><span data-stu-id="66f0c-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="66f0c-106">[Segítség a csatlakoztatott hálózati meghajtók hibaelhárításához](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="66f0c-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="66f0c-107">A tárak hálózati meghajtóként való hozzárendelése csak az Internet Explorer programban lehetséges, csak átmeneti és támogatott.</span><span class="sxs-lookup"><span data-stu-id="66f0c-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="66f0c-108">Ehelyett [szinkronizálja a SharePoint-fájlokat az új OneDrive szinkronizáló ügyféllel](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , amely tartalmaz [igény szerinti fájlokat](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="66f0c-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="66f0c-109">Belépés minden-a fájlokat-ban OneDrive nélkül használ helyi raktározás hely.</span><span class="sxs-lookup"><span data-stu-id="66f0c-109">Access all your files in OneDrive without using local storage space.</span></span>
  