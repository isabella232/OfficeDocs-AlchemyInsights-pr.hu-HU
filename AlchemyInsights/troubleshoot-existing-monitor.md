---
title: Meglévő monitor hibaelhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824581"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="e912b-102">Meglévő monitor hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="e912b-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="e912b-103">Az alábbi megoldásokkal elháríthatja a monitorok hibáit.</span><span class="sxs-lookup"><span data-stu-id="e912b-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="e912b-104">**A monitor megjelenítésének frissítése:**</span><span class="sxs-lookup"><span data-stu-id="e912b-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="e912b-105">Nyomja le egyszerre a következő billentyűket: Windows billentyű + Ctrl + Shift + B. Ez frissíti a kommunikációt a video-illesztőprogrammal.</span><span class="sxs-lookup"><span data-stu-id="e912b-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="e912b-106">A monitorok egy pillanatra villognak, és néhány másodperc múlva visszatérnek.</span><span class="sxs-lookup"><span data-stu-id="e912b-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="e912b-107">**A monitorok hardveres hibáinak elhárítása:**</span><span class="sxs-lookup"><span data-stu-id="e912b-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="e912b-108">Húzza ki a számítógépet a monitorhoz csatlakozó kábelt, és dugja be újra.</span><span class="sxs-lookup"><span data-stu-id="e912b-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="e912b-109">Leválaszthatja a nem alapvető eszközöket a pc-ről (például az adaptereket és a dokkolókat).</span><span class="sxs-lookup"><span data-stu-id="e912b-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="e912b-110">**Ha nemrég telepített egy frissítést a PC-jén, akkor visszaveheti a képernyő-illesztőprogramot:**</span><span class="sxs-lookup"><span data-stu-id="e912b-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="e912b-111">Válassza **a Start** gombot, írja be az **eszközkezelő** parancsot, és válassza az **Eszközkezelő lehetőséget** a találatok közül.</span><span class="sxs-lookup"><span data-stu-id="e912b-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="e912b-112">**Bontsa ki a Videokártyák szakaszt,** kattintson a jobb gombbal a videokártyára, és válassza a Tulajdonságok **parancsot.**</span><span class="sxs-lookup"><span data-stu-id="e912b-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="e912b-113">Lépjen az Illesztőprogram **lapra,** és válassza **az Illesztőprogram visszagörgetése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e912b-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="e912b-114">Megjegyzés: Ha ez nem érhető el vagy  szürkén jelenik meg, az alábbi lehetőségek közül a Nem lehetőséget választva lépjen a következő lépésre.</span><span class="sxs-lookup"><span data-stu-id="e912b-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="e912b-115">Előfordulhat, hogy a módosítások érvénybe léptéhez újra kell indítania a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="e912b-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="e912b-116">**Távolítsa el, majd telepítse újra a képernyő-illesztőprogramot:**</span><span class="sxs-lookup"><span data-stu-id="e912b-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="e912b-117">Válassza **a Start** gombot, írja be az **eszközkezelő** parancsot, és válassza az **Eszközkezelő lehetőséget** a találatok közül.</span><span class="sxs-lookup"><span data-stu-id="e912b-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="e912b-118">**Bontsa ki a Videokártyák szakaszt,** kattintson a jobb gombbal a videokártyára, és válassza az Eszköz eltávolítása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e912b-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="e912b-119">Jelölje be az Eszközillesztő-szoftver törlése **jelölőnégyzetet,** és válassza az Eltávolítás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e912b-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="e912b-120">Megjegyzés: Előfordulhat, hogy a rendszer a számítógép újraindítását kéri ebben a fázisban.</span><span class="sxs-lookup"><span data-stu-id="e912b-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="e912b-121">Az újraindítás előtt mindenképpen írja le a hátralévő utasításokat.</span><span class="sxs-lookup"><span data-stu-id="e912b-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="e912b-122">Nyissa meg ismét az Eszközkezelőt.</span><span class="sxs-lookup"><span data-stu-id="e912b-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="e912b-123">Bontsa ki **a Videokártyák szakaszt,** kattintson a jobb gombbal a videokártyára, és válassza az **Illesztőprogram frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e912b-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="e912b-124">Válassza **a Frissítési szoftver automatikus keresése lehetőséget,** és kövesse a telepítési utasításokat.</span><span class="sxs-lookup"><span data-stu-id="e912b-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>