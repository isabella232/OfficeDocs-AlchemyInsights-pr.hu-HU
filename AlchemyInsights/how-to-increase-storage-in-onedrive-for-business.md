---
title: A tárterület növelése a OneDrive vállalati verzióban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 676b17d47ee5071ed45e8d6022eaa82b51fc4d51
ms.sourcegitcommit: ad2d185aa9e08c27c4a1c4803b679cc4e6305703
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/16/2020
ms.locfileid: "48489009"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="9db5f-102">A tárterület növelése a OneDrive vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="9db5f-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="9db5f-103">Az új és meglévő OneDrive-felhasználók alapértelmezett tárterületének módosítása:</span><span class="sxs-lookup"><span data-stu-id="9db5f-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="9db5f-104">Nyissa meg a [OneDrive felügyeleti központ tárterület lapját](https://admin.onedrive.com/?v=StorageSettings), írjon be egy új összeget GB-ban, majd válassza a **Mentés**gombot.</span><span class="sxs-lookup"><span data-stu-id="9db5f-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), enter a new amount in GB, then select **Save**.</span></span>

<span data-ttu-id="9db5f-105">Ez a tárterület-beállítás minden olyan felhasználó esetében érvényes, akinek nincsenek meghatározott tárterület-korlátozásai.</span><span class="sxs-lookup"><span data-stu-id="9db5f-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="9db5f-106">Ha meg szeretné változtatni a tárterületet bizonyos felhasználók számára, használja a Microsoft PowerShellt.</span><span class="sxs-lookup"><span data-stu-id="9db5f-106">To change the storage space for specific users, use Microsoft PowerShell.</span></span> <span data-ttu-id="9db5f-107">Ebből a témakörből megtudhatja, hogy miként teheti ezt meg: a [felhasználók OneDrive-tárterületének módosítása a PowerShell használatával](https://docs.microsoft.com/onedrive/change-user-storage).</span><span class="sxs-lookup"><span data-stu-id="9db5f-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span></span>

<span data-ttu-id="9db5f-108">**Megjegyzés**: úgy tűnik, nincs olyan csomag, amely korlátlan tárterületet tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="9db5f-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="9db5f-109">Az egyes csomagokhoz tartozó tárterületekről a [OneDrive vállalati verzió szolgáltatás leírása](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="9db5f-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>
  
<span data-ttu-id="9db5f-110">Ha növelni szeretné tárterületét a OneDrive vállalati verzióban, válassza ki azt az előfizetést, amely a **2 vagy az** **Office 365 E3**csomagot tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="9db5f-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 E3**.</span></span>
  
<span data-ttu-id="9db5f-111">A csomagok módosításához a felügyeleti központban lépjen a termékek **számlázása** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) lapra, válassza ki a módosítani kívánt előfizetést, majd válassza a **szervezete számára ajánlott frissítések megtekintése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9db5f-111">To change plans, in the admin center, go to the **Billing** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) page, select the subscription to change, then choose **View upgrades recommended for your org**.</span></span>
  
<span data-ttu-id="9db5f-112">A csomagok és a OneDrive vállalati verzió tárterületének módosításáról további információt a váltás [másik csomagra](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) és a [OneDrive vállalati verzió szolgáltatás leírása](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="9db5f-112">For more information on changing plans and OneDrive for Business storage, see [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) and the [OneDrive for Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>