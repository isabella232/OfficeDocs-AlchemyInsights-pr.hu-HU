---
title: Lemezterület felszabadítja a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036587"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="fa400-102">Lemezterület felszabadítja a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="fa400-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="fa400-103">A következő két lehetőséggel szabadíthat fel lemezterületet a Windowsban:</span><span class="sxs-lookup"><span data-stu-id="fa400-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="fa400-104">Szabadíthat fel lemezterületet a Windows 10-ben.</span><span class="sxs-lookup"><span data-stu-id="fa400-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="fa400-105">Tárterületet szabadíthat fel a Windows 10-frissítések számára külső tárolóeszköz segítségével.</span><span class="sxs-lookup"><span data-stu-id="fa400-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="fa400-106">Ha a Lemezkarbantartó használata után továbbra is kevés a lemezterület, akkor lehet, hogy a Temp mappa gyorsan kitölti a Microsoft Store által használt alkalmazásfájlokat (.appx).</span><span class="sxs-lookup"><span data-stu-id="fa400-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="fa400-107">A probléma megoldásához állítsa alaphelyzetbe az Áruházat, ürítse ki az Áruház gyorsítótárát, majd futtassa a Windows Update hibaelhárítót.</span><span class="sxs-lookup"><span data-stu-id="fa400-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="fa400-108">Mielőtt továbblép, győződjön meg arról, hogy a Microsoft Store be van zárva.</span><span class="sxs-lookup"><span data-stu-id="fa400-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="fa400-109">**1. lépés: A Microsoft Store alaphelyzetbe állítása**</span><span class="sxs-lookup"><span data-stu-id="fa400-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="fa400-110">**Megjegyzés** Ez véglegesen törli az alkalmazásadatokat az eszközön, beleértve a beállításokat és a bejelentkezési adatokat.</span><span class="sxs-lookup"><span data-stu-id="fa400-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="fa400-111">Válassza a **Start**  >  **Settings**  >  **Apps apps**&  >  **gombra.**</span><span class="sxs-lookup"><span data-stu-id="fa400-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="fa400-112">Az appok listájában keresse meg és válassza a Microsoft Store lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fa400-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="fa400-113">Válassza **a Speciális beállítások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="fa400-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="fa400-114">Görgessen le, és **válassza az Alaphelyzet**, majd az **Alaphelyzetbe állítás megerősítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="fa400-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="fa400-115">**2. lépés: A Microsoft Store gyorsítótárának kiürítése**</span><span class="sxs-lookup"><span data-stu-id="fa400-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="fa400-116">A Windows billentyű + R billentyűkombinációt lenyomva nyissa meg a Futtatás párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="fa400-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="fa400-117">Írja be a wsreset.exe, és válassza az **OK gombot.**</span><span class="sxs-lookup"><span data-stu-id="fa400-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="fa400-118">Megnyílik egy üres parancssorablak.</span><span class="sxs-lookup"><span data-stu-id="fa400-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="fa400-119">Körülbelül 10 másodperc elteltével az ablak bezárul, és az Áruház automatikusan megnyílik.</span><span class="sxs-lookup"><span data-stu-id="fa400-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="fa400-120">**3. lépés: A Windows Update alaphelyzetbe állítása**</span><span class="sxs-lookup"><span data-stu-id="fa400-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="fa400-121">Válassza **a Start**  >  **Settings** Update & Biztonsági hibaelhárítás  >    >  **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="fa400-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="fa400-122">Görgessen le, és válassza a **Windows Update** listában a Hibaelhárító **futtatása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="fa400-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="fa400-123">Indítsa újra a számítógépet, és ellenőrizze, hogy továbbra is tapasztalja-e a problémát.</span><span class="sxs-lookup"><span data-stu-id="fa400-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

