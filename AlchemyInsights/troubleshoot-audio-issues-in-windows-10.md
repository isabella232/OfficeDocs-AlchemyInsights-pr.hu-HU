---
title: Hanggal kapcsolatos problémák elhárítása a Windows 10 rendszerben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796171"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="111f1-102">A Windows 10 hangproblémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="111f1-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="111f1-103">**A hang hibaelhárítójának futtatása**</span><span class="sxs-lookup"><span data-stu-id="111f1-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="111f1-104">Lehet, hogy a hang hibaelhárító automatikusan meg tudja oldani a hangproblémákat:</span><span class="sxs-lookup"><span data-stu-id="111f1-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="111f1-105">Kattintson a Start gombra, írja be a **Hibaelhárítás**típust, majd válassza ki a **hibaelhárítást**az eredménylistából. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="111f1-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="111f1-106">Válassza az **audió** > lejátszása**a hibaelhárítót**.</span><span class="sxs-lookup"><span data-stu-id="111f1-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="111f1-107">**Ellenõrizze a kábeleket, a hangerőt, a hangszórókat és a fejhallgatót**</span><span class="sxs-lookup"><span data-stu-id="111f1-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="111f1-108">Ellenőrizze a hangszóró és fejhallgató csatlakozásait laza kábeleknél, és győződjön meg arról, hogy a csatlakozó csatlakoztatva van a megfelelő aljzathoz.</span><span class="sxs-lookup"><span data-stu-id="111f1-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="111f1-109">Ellenőrizze a tápkábelt és a hangerőt, és próbálja meg a hangerőszabályzás elforgatását.</span><span class="sxs-lookup"><span data-stu-id="111f1-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="111f1-110">Egyes hangszórók és alkalmazások saját hangerőszabályzókkal rendelkeznek, és esetleg ellenőrizni kell mindet, hogy biztosan a megfelelő szinteken legyenek.</span><span class="sxs-lookup"><span data-stu-id="111f1-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="111f1-111">Próbáljon egy másik USB-porton keresztül kapcsolódni.</span><span class="sxs-lookup"><span data-stu-id="111f1-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="111f1-112">**Megjegyzés:** Ne feledje, hogy a hangszórók nem működnek, ha a fejhallgatót csatlakoztatta.</span><span class="sxs-lookup"><span data-stu-id="111f1-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="111f1-113">**Eszközkezelő ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="111f1-113">**Check Device Manager**</span></span>

<span data-ttu-id="111f1-114">Annak érdekében, hogy az illesztőprogramok naprakész:</span><span class="sxs-lookup"><span data-stu-id="111f1-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="111f1-115">Kiválaszt **elkezd**, típus **berendezés igazgató**, aztán kiválaszt **berendezés igazgató** -ból oldalra dől-ból eredmények.</span><span class="sxs-lookup"><span data-stu-id="111f1-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="111f1-116">A **hang-, video-és játékvezérlők**területen válassza ki a hangkártyát, nyissa meg, jelölje ki az **illesztőprogram** lapot, és válassza az **Illesztőprogram frissítése**-t.</span><span class="sxs-lookup"><span data-stu-id="111f1-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="111f1-117">**Megjegyzés:** Ha a Windows nem talál új illesztőprogramot, keressen egyet az eszköz gyártójának webhelyén, és kövesse azok utasításait.</span><span class="sxs-lookup"><span data-stu-id="111f1-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="111f1-118">**Telepítse újra az illesztőprogramot**</span><span class="sxs-lookup"><span data-stu-id="111f1-118">**Reinstall the driver**</span></span>

<span data-ttu-id="111f1-119">Ha nem tudja frissíteni az Eszközkezelőt vagy új illesztőprogramot talál a gyártó webhelyén, próbálkozzon az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="111f1-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="111f1-120">Az Eszközkezelőben kattintson a jobb gombbal (vagy nyomja meg és tartsa lenyomva) az audio-illesztőprogramot, és válassza az **Eltávolítás**.</span><span class="sxs-lookup"><span data-stu-id="111f1-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="111f1-121">Indítsa újra az eszközt, és a Windows megkísérli az illesztõprogram újratelepítését.</span><span class="sxs-lookup"><span data-stu-id="111f1-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="111f1-122">Ha az illesztőprogram újratelepítése nem működik, próbálja meg a Windows operációs rendszer általános audio-illesztőprogramját használni.</span><span class="sxs-lookup"><span data-stu-id="111f1-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="111f1-123">Az Eszközkezelőben kattintson a jobb gombbal (vagy nyomja meg és tartsa lenyomva) az audio-illesztőprogramot > **Update illesztőprogram** > a Sajátgép**a** > számítógépen,**hadd válasszon egy listát az eszközillesztők a számítógépen**, válasszuk a **High Definition Audio eszközt**, válassza a **Next**, és kövesse az utasításokat, hogy telepítse azt.</span><span class="sxs-lookup"><span data-stu-id="111f1-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="111f1-124">**Az alapértelmezett eszköz beállítása**</span><span class="sxs-lookup"><span data-stu-id="111f1-124">**Set the default device**</span></span>

<span data-ttu-id="111f1-125">Ha USB-vagy HDMI-kábellel csatlakozik egy audioeszközhöz, lehet, hogy az eszközt alapértelmezettként kell beállítani:</span><span class="sxs-lookup"><span data-stu-id="111f1-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="111f1-126">Válassza a **Start**-t, írja be a **hang**, majd válassza a **hang** vagy a **rendszerhangok módosítása** listát az eredménylistából.</span><span class="sxs-lookup"><span data-stu-id="111f1-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="111f1-127">A **Lejátszás** lapon jelöljön ki egy eszközt, jelölje be az **alapértelmezés**választógombot, majd kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="111f1-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

