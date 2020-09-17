---
title: A tárterület növelése a OneDrive vállalati verzióban
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 53eabf6c87dead3b7309c7da1f8a590940127169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780097"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="1432c-102">A tárterület növelése a OneDrive vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="1432c-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="1432c-103">Az új és meglévő OneDrive-felhasználók alapértelmezett tárterületének módosítása:</span><span class="sxs-lookup"><span data-stu-id="1432c-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="1432c-104">Nyissa meg a [OneDrive felügyeleti központ tárterület lapját](https://admin.onedrive.com/?v=StorageSettings), és írjon be egy új összeget GB-ban.</span><span class="sxs-lookup"><span data-stu-id="1432c-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="1432c-105">Ez a tárterület-beállítás minden olyan felhasználó esetében érvényes, akinek nincsenek meghatározott tárterület-korlátozásai.</span><span class="sxs-lookup"><span data-stu-id="1432c-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="1432c-106">Ha módosítani szeretné bizonyos felhasználók tárterületét, a Microsoft PowerShellt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="1432c-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="1432c-107">Ebből a témakörből megtudhatja, hogy miként teheti ezt meg: a [felhasználók OneDrive-tárterületének módosítása a PowerShell használatával](https://go.microsoft.com/fwlink/?linkid=866402).</span><span class="sxs-lookup"><span data-stu-id="1432c-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="1432c-108">**Megjegyzés**: úgy tűnik, nincs olyan csomag, amely korlátlan tárterületet tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="1432c-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="1432c-109">Az egyes csomagokhoz tartozó tárterületekről a [OneDrive vállalati verzió szolgáltatás leírása](https://go.microsoft.com/fwlink/p/?LinkID=826071)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="1432c-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="1432c-110">Ha növelni szeretné tárterületét a OneDrive vállalati verzióban, válassza ki azt az előfizetést, amely a OneDrive vállalati verzió vagy **az** **Office 365 Enterprise E3**csomagját tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="1432c-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="1432c-111">A csomagok módosításához a Microsoft 365 felügyeleti központban lépjen a termékek **számlázása** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** lapra, jelölje ki a módosítani kívánt előfizetést, és válassza a **frissítés** fület.</span><span class="sxs-lookup"><span data-stu-id="1432c-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="1432c-112">A csomagok és a OneDrive vállalati verzió tárterületének váltásáról további információt a [Váltás másik Microsoft 365 vállalati verziós csomagra](https://go.microsoft.com/fwlink/?LinkId=2031117) és a [OneDrive vállalati verzió szolgáltatás leírása](https://go.microsoft.com/fwlink/p/?LinkId-2031122)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="1432c-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>