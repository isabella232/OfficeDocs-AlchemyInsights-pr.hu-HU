---
title: A tárhely növelése a OneDrive Vállalati verzióban
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: adee1c5d1ffc23f54580549ab666ee8fac579263
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2020
ms.locfileid: "44063043"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="3c7f2-102">A tárhely növelése a OneDrive Vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="3c7f2-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="3c7f2-103">Az új és meglévő OneDrive-felhasználók alapértelmezett tárhelyének módosítása:</span><span class="sxs-lookup"><span data-stu-id="3c7f2-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="3c7f2-104">Nyissa meg [a OneDrive Felügyeleti központ Tárolás lapját,](https://admin.onedrive.com/?v=StorageSettings)és adjon meg egy új összeget GB-ban.</span><span class="sxs-lookup"><span data-stu-id="3c7f2-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="3c7f2-105">Ez a tárhelybeállítás minden olyan felhasználóra vonatkozik, akiknek nem adott tárhelykorlátokat állított be.</span><span class="sxs-lookup"><span data-stu-id="3c7f2-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="3c7f2-106">Az adott felhasználók tárhelyének módosításához a Microsoft PowerShell t kell használnia.</span><span class="sxs-lookup"><span data-stu-id="3c7f2-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="3c7f2-107">Ennek módjáról a Felhasználók [OneDrive-tárhelyének módosítása a PowerShell használatával (A felhasználók OneDrive-tárhelyének módosítása) témakörben talál.](https://go.microsoft.com/fwlink/?linkid=866402)</span><span class="sxs-lookup"><span data-stu-id="3c7f2-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="3c7f2-108">**Megjegyzés:** Úgy néz ki, hogy nincs olyan csomagja, amely korlátlan tárhelyet tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="3c7f2-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="3c7f2-109">Az egyes sémákhoz kapcsolódó tárhelyről a [OneDrive Vállalati verzió szolgáltatás leírásában](https://go.microsoft.com/fwlink/p/?LinkID=826071)talál további információt.</span><span class="sxs-lookup"><span data-stu-id="3c7f2-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="3c7f2-110">A OneDrive Vállalati verzióban tárolt tárhely növeléséhez válasszon olyan előfizetést, amely tartalmazza a **OneDrive Vállalati csomag 2-t** vagy az **Office 365 Nagyvállalati E3 csomagot.**</span><span class="sxs-lookup"><span data-stu-id="3c7f2-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="3c7f2-111">A csomagok módosításához a Microsoft 365 Felügyeleti központban nyissa meg a **[Termékek](https://go.microsoft.com/fwlink/p/?linkid=842054)** **számlázása** \> lapot, válassza a módosítani kívánt előfizetést, majd válassza a **Frissítés** lapot.</span><span class="sxs-lookup"><span data-stu-id="3c7f2-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="3c7f2-112">A csomagok és a OneDrive Vállalati verzió tárhelyének váltásáról a [Váltás egy másik Microsoft 365 vállalati verziós csomagra](https://go.microsoft.com/fwlink/?LinkId=2031117) című témakörben és a [OneDrive Vállalati verzió szolgáltatás leírása című témakörben](https://go.microsoft.com/fwlink/p/?LinkId-2031122)talál.</span><span class="sxs-lookup"><span data-stu-id="3c7f2-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>