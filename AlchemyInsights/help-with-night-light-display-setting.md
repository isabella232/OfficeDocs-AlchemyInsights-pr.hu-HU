---
title: Segítség az éjszakai fény megjelenítési beállításával
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404663"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="b0072-102">Segítség az éjszakai fény megjelenítési beállításával</span><span class="sxs-lookup"><span data-stu-id="b0072-102">Help with the night light display setting</span></span>

<span data-ttu-id="b0072-103">Az éjszakai megjelenítés beállításairól további információt A kijelző beállítása éjszakai megjelenítésre [Windows 10-ben.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="b0072-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="b0072-104">Ha az éjszakai fény beállításai szürkén jelennek meg a Beállítások lapon, ellenőrizze a kijelző illesztőprogramját:</span><span class="sxs-lookup"><span data-stu-id="b0072-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="b0072-105">Kattintson a tálcán a keresőmezőbe, írja  be az **Eszközkezelő** parancsot, majd a találatok között válassza az Eszközkezelő lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b0072-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="b0072-106">**Bontsa ki a videokártyákat.**</span><span class="sxs-lookup"><span data-stu-id="b0072-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="b0072-107">Az éjszakai fény szolgáltatás sajnos nem érhető el, ha az eszköz DisplayLink illesztőprogramot vagy egyszerű kijelző-illesztőprogramot használ.</span><span class="sxs-lookup"><span data-stu-id="b0072-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="b0072-108">Az éjszakai fény funkció a legújabb grafikus technológiát használja, ezért előfordulhat, hogy frissítenie kell a kijelző illesztőprogramját:</span><span class="sxs-lookup"><span data-stu-id="b0072-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="b0072-109">A frissítéseket a **Start**  >  **Settings** Update & Windows Update Check for Updates  >    >  **(Biztonsági Windows**  >  **Update-frissítések** keresése) lapon ellenőrizheti.</span><span class="sxs-lookup"><span data-stu-id="b0072-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="b0072-110">VAGY</span><span class="sxs-lookup"><span data-stu-id="b0072-110">OR</span></span>

- <span data-ttu-id="b0072-111">A hardver gyártójának támogatási webhelyén manuálisan töltse le és telepítse a legújabb illesztőprogramokat.</span><span class="sxs-lookup"><span data-stu-id="b0072-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="b0072-112">Éjszakai fény alaphelyzetbe állítása a beállításjegyzékben</span><span class="sxs-lookup"><span data-stu-id="b0072-112">Reset night light in the registry</span></span>

<span data-ttu-id="b0072-113">Ha a képernyőillesztő frissítése nem működik, előfordulhat, hogy alaphelyzetbe kell állítania az éjszakai fényt a beállításjegyzékben.</span><span class="sxs-lookup"><span data-stu-id="b0072-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="b0072-114">**Figyelem:** Ez a hibaelhárítási lépés csak haladó felhasználóknak ajánlott.</span><span class="sxs-lookup"><span data-stu-id="b0072-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="b0072-115">Ha helytelenül módosítja a beállításjegyzéket, komoly problémák léphetnek fel.</span><span class="sxs-lookup"><span data-stu-id="b0072-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="b0072-116">A további védelem érdekében a módosítás előtt biztonsági mentést kell a beállításjegyzékről, hogy probléma esetén visszaállítsa azt.</span><span class="sxs-lookup"><span data-stu-id="b0072-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="b0072-117">Írja be a **keresőmezőbe a regedit**, majd a találatok között **a** Beállításszerkesztő lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b0072-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="b0072-118">Ugrás a következő beállításkulcsra:</span><span class="sxs-lookup"><span data-stu-id="b0072-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="b0072-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="b0072-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="b0072-120">Exportálja, majd törölje a következő alkulcsot:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="b0072-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="b0072-121">Exportálja, majd törölje a következő alkulcsot:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="b0072-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="b0072-122">Indítsa újra a Windowst, és ellenőrizze, hogy elérhetők-e az éjszakai fény beállításai.</span><span class="sxs-lookup"><span data-stu-id="b0072-122">Restart Windows and verify if the night light options are available.</span></span>


