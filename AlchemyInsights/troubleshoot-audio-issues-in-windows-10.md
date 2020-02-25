---
title: Hangproblémák a Windows 10-ben – problémamegoldás
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
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265018"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="ab3aa-102">Hangproblémák elhárítása a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="ab3aa-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="ab3aa-103">**A hanghiba-elhárító futtatása**</span><span class="sxs-lookup"><span data-stu-id="ab3aa-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="ab3aa-104">Nyissa meg a [Hibaelhárítási beállítások at](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="ab3aa-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="ab3aa-105">Válassza **a Hang** > **lejátszása A hibaelhárító futtatása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ab3aa-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="ab3aa-106">**Az alapértelmezett eszköz beállítása**</span><span class="sxs-lookup"><span data-stu-id="ab3aa-106">**Set the default device**</span></span>

<span data-ttu-id="ab3aa-107">Ha USB vagy HDMI rendszerrel csatlakozik egy hangeszközhöz, előfordulhat, hogy az eszközt kell alapértelmezettként beállítania:</span><span class="sxs-lookup"><span data-stu-id="ab3aa-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="ab3aa-108">Nyissa meg a **Hang indítása** > **lehetőséget,** majd válassza a **Hang** vagy **a Rendszerhangok módosítása** lehetőséget az eredmények listájából.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="ab3aa-109">A **Lejátszás** lapon jelöljön ki egy eszközt, válassza az **Alapértelmezett beállítás**lehetőséget, majd az **OK**gombot.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="ab3aa-110">**Kábelek, hangerő, hangszórók és fejhallgatók ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="ab3aa-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="ab3aa-111">Ellenőrizze a hangszóró és a fejhallgató csatlakozóit, hogy nincsenek-e laza kábelek, és győződjön meg arról, hogy a megfelelő csatlakozóhoz vannak csatlakoztatva.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="ab3aa-112">Ellenőrizze a teljesítmény és a hangerő szintjét, és próbálja meg az összes hangerőszabályzót felfelé fordítani.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="ab3aa-113">Egyes hangszórók és alkalmazások saját hangerőszabályzóval rendelkeznek; Lehet, hogy ellenőrizni őket, hogy megbizonyosodjon arról, hogy ők a megfelelő szinten.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="ab3aa-114">Próbáljon meg másik USB-porton keresztül csatlakozni.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="ab3aa-115">**Megjegyzés: Ne feledje,** hogy a hangszórók nem működnek, ha a fejhallgató csatlakoztatva van.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="ab3aa-116">**Eszközkezelő ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="ab3aa-116">**Check Device Manager**</span></span>

<span data-ttu-id="ab3aa-117">Annak biztosítása, hogy az illesztőprogramok naprakészek legyenek:</span><span class="sxs-lookup"><span data-stu-id="ab3aa-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="ab3aa-118">Válassza a **Start**lehetőséget , írja be **az Eszközkezelő**parancsot , majd az Eredménylistában válassza az **Eszközkezelő** elemet.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="ab3aa-119">A **Hang-, video- és játékvezérlők**csoportban jelölje ki a hangkártyát, nyissa meg, válassza az **Illesztőprogram** lapot, és válassza az **Illesztőprogram frissítése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="ab3aa-120">**Megjegyzés:** Ha a Windows nem talál új illesztőprogramot, keressen egyet az eszköz gyártójának webhelyén, és kövesse az utasításokat.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="ab3aa-121">**Az illesztőprogram újratelepítése**</span><span class="sxs-lookup"><span data-stu-id="ab3aa-121">**Reinstall the driver**</span></span>

<span data-ttu-id="ab3aa-122">Ha nem tud frissíteni az Eszközkezelőn keresztül, vagy nem talál új illesztőprogramot a gyártó webhelyén, próbálkozzon az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="ab3aa-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="ab3aa-123">Az Eszközkezelőben kattintson a jobb gombbal (vagy tartsa nyomva) az audio-illesztőprogramot, és válassza **az Eltávolítás parancsot.**</span><span class="sxs-lookup"><span data-stu-id="ab3aa-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="ab3aa-124">Indítsa újra az eszközt, és a Windows megpróbálja újratelepíteni az illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="ab3aa-125">Ha az illesztőprogram újratelepítése nem működik, próbálja meg használni a Windows általános hangillesztőjét.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="ab3aa-126">Az Eszközkezelőben kattintson a jobb gombbal (vagy tartsa lenyomva) az audio-illesztőprogramot > frissítse az **illesztőprogram-szoftvert** > A számítógép böngészése**illesztőprogram-szoftverhez:** > Válasszam ki a**számítógép eszközillesztőinek listájából,** válassza a **Nagy felbontású hangeszköz**lehetőséget, válassza a **Tovább**lehetőséget, és kövesse a telepítéshez szükséges utasításokat.</span><span class="sxs-lookup"><span data-stu-id="ab3aa-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
