---
title: Üzenetek automatikus áthelyezésének megállítása az archívumba
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525104"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="680a2-102">Üzenetek automatikus áthelyezésének megállítása az archívumba</span><span class="sxs-lookup"><span data-stu-id="680a2-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="680a2-103">Adatmegőrzési házirend használata esetén módosíthatja a házirend adatmegőrzési korát úgy, hogy az üzenetek ne archiválják automatikusan az üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="680a2-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="680a2-104">Ezt a következőképpen teheti meg:</span><span class="sxs-lookup"><span data-stu-id="680a2-104">Here's how:</span></span>

1. <span data-ttu-id="680a2-105">Az [Exchange Felügyeleti központban válassza](https://go.microsoft.com/fwlink/?linkid=2059104) **ki a megfelelőségi kezelési adatmegőrzési**  >  **címkéket.**</span><span class="sxs-lookup"><span data-stu-id="680a2-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="680a2-106">Keresse meg az Áthelyezés archívumba adatmegőrzési címkét.</span><span class="sxs-lookup"><span data-stu-id="680a2-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="680a2-107">Az adatmegőrzési címkében módosítsa az adatmegőrzési időszakot (archiválási időszakot) úgy, hogy soha ne állítsa le az elemek adatmegőrzési házirend által való automatikus archiválását. </span><span class="sxs-lookup"><span data-stu-id="680a2-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="680a2-108">Ez módosítja az összes olyan postaláda archiválási beállítását, amelyekre ez az adatmegőrzési címke vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="680a2-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
