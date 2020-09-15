---
title: A meglévő monitor hibaelhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690713"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="c5388-102">Meglévő monitor hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="c5388-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="c5388-103">Próbálkozzon ezekkel a megoldásokkal a monitor hibaelhárításához.</span><span class="sxs-lookup"><span data-stu-id="c5388-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="c5388-104">**A monitor megjelenítésének frissítése:**</span><span class="sxs-lookup"><span data-stu-id="c5388-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="c5388-105">Nyomja le a következő billentyűket egyszerre: Windows billentyű + CTRL + SHIFT + B. Ez frissíti a grafikus illesztőprogrammal folytatott kommunikációt.</span><span class="sxs-lookup"><span data-stu-id="c5388-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="c5388-106">A monitorok egy pillanatra villognak, és néhány másodperc elteltével visszatérhetnek.</span><span class="sxs-lookup"><span data-stu-id="c5388-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="c5388-107">**Monitor hardverének hibaelhárítása:**</span><span class="sxs-lookup"><span data-stu-id="c5388-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="c5388-108">Húzza ki a SZÁMÍTÓGÉPét a monitorhoz csatlakozó kábelt, és csatlakoztassa újra a monitorhoz.</span><span class="sxs-lookup"><span data-stu-id="c5388-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="c5388-109">Húzzon le minden nem alapvető eszközt a SZÁMÍTÓGÉPRŐL (például adapterek vagy dokkok).</span><span class="sxs-lookup"><span data-stu-id="c5388-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="c5388-110">**Ha nemrég telepített egy frissítést a SZÁMÍTÓGÉPére, visszaállíthatja a képernyő-illesztőprogramot:**</span><span class="sxs-lookup"><span data-stu-id="c5388-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="c5388-111">Válassza a **Start**gombot, írja be az **Eszközkezelőt**, és az eredményből válassza az **Eszközkezelő** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c5388-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="c5388-112">Bontsa **ki a videokártyák** szakaszt, kattintson a jobb gombbal a videokártyához, ands válassza a **Tulajdonságok parancsot**.</span><span class="sxs-lookup"><span data-stu-id="c5388-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="c5388-113">Lépjen az **illesztőprogram** lapra, és válassza az **illesztőprogram visszaállítása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c5388-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="c5388-114">Megjegyzés: Ha ez a funkció nem érhető el, vagy szürkén jelenik meg, válassza a **nem** lehetőséget az alábbi lehetőségek közül a következő lépésre való ugráshoz.</span><span class="sxs-lookup"><span data-stu-id="c5388-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="c5388-115">Előfordulhat, hogy a módosítások életbe léptetéséhez újra kell indítania a GÉPET.</span><span class="sxs-lookup"><span data-stu-id="c5388-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="c5388-116">**A képernyő-illesztőprogram eltávolítása és újratelepítése:**</span><span class="sxs-lookup"><span data-stu-id="c5388-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="c5388-117">Válassza a **Start**gombot, írja be az **Eszközkezelőt**, és az eredményből válassza az **Eszközkezelő** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c5388-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="c5388-118">Bontsa **ki a videokártyák** szakaszt, kattintson a jobb gombbal a videokártyához, ands válassza az **eszköz eltávolítása**parancsot.</span><span class="sxs-lookup"><span data-stu-id="c5388-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="c5388-119">Jelölje be az **eszközhöz tartozó illesztőprogram törlése** elem melletti jelölőnégyzetet, és válassza az **Eltávolítás**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c5388-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="c5388-120">Megjegyzés: Előfordulhat, hogy a rendszer kéri a számítógép újraindítását ebben a fázisban.</span><span class="sxs-lookup"><span data-stu-id="c5388-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="c5388-121">Mielőtt újraindul, ügyeljen rá, hogy írja le a fennmaradó utasításokat.</span><span class="sxs-lookup"><span data-stu-id="c5388-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="c5388-122">Nyissa meg ismét az Eszközkezelőt.</span><span class="sxs-lookup"><span data-stu-id="c5388-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="c5388-123">Bontsa **ki a videokártyák** szakaszt, kattintson a jobb gombbal a videokártyához, és válassza az **Illesztőprogram frissítése**parancsot.</span><span class="sxs-lookup"><span data-stu-id="c5388-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="c5388-124">Válassza az **Illesztőprogram frissítése automatikus keresése** lehetőséget, és kövesse a telepítési útmutatót.</span><span class="sxs-lookup"><span data-stu-id="c5388-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>