---
title: Hangproblémák elhárítása a Windows 10-ben
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833293"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="9289c-102">Hangproblémák elhárítása a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="9289c-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="9289c-103">**A hanghibát hibaelhárító futtatása**</span><span class="sxs-lookup"><span data-stu-id="9289c-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="9289c-104">Nyissa meg [a Hibaelhárítási beállításokat.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="9289c-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="9289c-105">Válassza **a**  >  **Hanglejátszás futtassa a hibaelhárítót lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9289c-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="9289c-106">**Az alapértelmezett eszköz beállítása**</span><span class="sxs-lookup"><span data-stu-id="9289c-106">**Set the default device**</span></span>

<span data-ttu-id="9289c-107">Ha USB-n vagy HDMI-n keresztül csatlakozik egy hangeszközhöz, előfordulhat, hogy az eszközt alapértelmezettként kell beállítania:</span><span class="sxs-lookup"><span data-stu-id="9289c-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="9289c-108">Nyissa **meg** a Start Hang menüt, majd a találatok listájában válassza a Hang vagy a  >  Rendszerhangok módosítása lehetőséget.  </span><span class="sxs-lookup"><span data-stu-id="9289c-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="9289c-109">A Lejátszás **lapon** jelöljön ki egy eszközt, válassza **az** Alapértelmezett gombra, majd az OK **gombot.**</span><span class="sxs-lookup"><span data-stu-id="9289c-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="9289c-110">**A kábelek, a hangerő, a hangszórók és a fejhallgatók ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="9289c-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="9289c-111">Ellenőrizze, hogy a hangszóró és a fejhallgató kábelei vannak-e lazán, és győződjön meg arról, hogy a megfelelő csatlakozóhoz vannak csatlakoztatva.</span><span class="sxs-lookup"><span data-stu-id="9289c-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="9289c-112">Ellenőrizze a tápellátást és a hangerő szintjét, és próbálja meg felfelé forgatni az összes hangerővezérlőt.</span><span class="sxs-lookup"><span data-stu-id="9289c-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="9289c-113">Egyes hangszórók és alkalmazások saját hangerővezérlővel is rendelkezik; lehet, hogy mindegyiket ellenőriznie kell, hogy a megfelelő szinten vannak-e.</span><span class="sxs-lookup"><span data-stu-id="9289c-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="9289c-114">Próbáljon meg másik USB-portot használni a csatlakozáshoz.</span><span class="sxs-lookup"><span data-stu-id="9289c-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="9289c-115">**Megjegyzés:** Ne feledje, hogy előfordulhat, hogy a hangszórók nem működnek, ha a fejhallgató csatlakoztatva van.</span><span class="sxs-lookup"><span data-stu-id="9289c-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="9289c-116">**Az Eszközkezelő ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="9289c-116">**Check Device Manager**</span></span>

<span data-ttu-id="9289c-117">Annak érdekében, hogy az illesztőprogramok naprakészek-e:</span><span class="sxs-lookup"><span data-stu-id="9289c-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="9289c-118">Válassza **a Start** gombot,  írja be az **Eszközkezelő**, majd a találatok listájában válassza az Eszközkezelő lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="9289c-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="9289c-119">A **Hang-, video-** és játékvezérlők alatt válassza ki  a hangkártyát, nyissa meg, válassza az Illesztőprogram fület, majd az **Illesztőprogram frissítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9289c-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="9289c-120">**Megjegyzés:** Ha a Windows nem talál új illesztőprogramot, keressen egyet az eszköz gyártójának webhelyén, és kövesse az ott található útmutatást.</span><span class="sxs-lookup"><span data-stu-id="9289c-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="9289c-121">**Az illesztőprogram újratelepítése**</span><span class="sxs-lookup"><span data-stu-id="9289c-121">**Reinstall the driver**</span></span>

<span data-ttu-id="9289c-122">Ha nem tud az Eszközkezelőn keresztül frissíteni, vagy új illesztőprogramot keres a gyártó webhelyén, próbálkozzon az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="9289c-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="9289c-123">Az Eszközkezelőben kattintson a jobb gombbal a hangillesztő illesztőprogramra (vagy tartsa nyomva), és válassza az Eltávolítás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9289c-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="9289c-124">Indítsa újra az eszközt, és a Windows megpróbálja újratelepíteni az illesztőprogramot.</span><span class="sxs-lookup"><span data-stu-id="9289c-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="9289c-125">Ha az illesztőprogram újratelepítése nem működik, próbálkozzon a Windows általános hangillesztőjével.</span><span class="sxs-lookup"><span data-stu-id="9289c-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="9289c-126">Az Eszközkezelőben kattintson a jobb gombbal a hangillesztőprogramra (vagy tartsa nyomva), > Illesztőprogram frissítése: Tallózással keresse meg a számítógépen az illesztőprogramokat: Válasszon a számítógépen található illesztőprogramok listájából, válassza a High Definition Audio Device (Nagy felbontású hangeszköz) lehetőséget, válassza a Tovább gombot, és kövesse a telepítési  >    >  útmutatót.  </span><span class="sxs-lookup"><span data-stu-id="9289c-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
