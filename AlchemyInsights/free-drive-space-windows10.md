---
title: Lemezterület felszabadítása a Windows 10 rendszerben
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505358"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="ffab8-102">Lemezterület felszabadítása a Windows 10 rendszerben</span><span class="sxs-lookup"><span data-stu-id="ffab8-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="ffab8-103">Alább bemutatunk két lehetőséget arra, hogyan szabadíthat fel lemezterületet a Windowsban:</span><span class="sxs-lookup"><span data-stu-id="ffab8-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="ffab8-104">Felszabadíthat lemezterületet a Windows 10-ben.</span><span class="sxs-lookup"><span data-stu-id="ffab8-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="ffab8-105">Külső tárolóeszköz segítségével felszabadíthat tárterületet a Windows 10 frissítései számára.</span><span class="sxs-lookup"><span data-stu-id="ffab8-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="ffab8-106">Ha a Lemezkarbantartó használata után is kevés a szabad lemezterület, előfordulhat, hogy a Temp mappában gyorsan összegyűlnek a Microsoft Store által használt alkalmazásfájlok (.appx).</span><span class="sxs-lookup"><span data-stu-id="ffab8-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="ffab8-107">A probléma elhárításához állítsa alaphelyzetbe a Store-t, ürítse ki a Store gyorsítótárát, majd futtassa a Windows Update hibaelhárítóját.</span><span class="sxs-lookup"><span data-stu-id="ffab8-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="ffab8-108">Ügyeljen arra, hogy az alábbi lépések elvégzése előtt bezárja a Microsoft Store-t.</span><span class="sxs-lookup"><span data-stu-id="ffab8-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="ffab8-109">**1. lépés: A Microsoft Store alaphelyzetbe állítása**</span><span class="sxs-lookup"><span data-stu-id="ffab8-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="ffab8-110">**Megjegyzés:** Ez a művelet véglegesen törli az eszközön levő alkalmazásadatokat, beleértve a személyes beállításokat és a bejelentkezési adatokat is.</span><span class="sxs-lookup"><span data-stu-id="ffab8-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="ffab8-111">Válassza a **Start** > **Gépház** > **Alkalmazások** > **Alkalmazások és szolgáltatások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ffab8-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="ffab8-112">Keresse meg és jelölje ki a Microsoft Store-t az alkalmazások listáján.</span><span class="sxs-lookup"><span data-stu-id="ffab8-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="ffab8-113">Válassza a **Speciális beállítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ffab8-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="ffab8-114">Görgessen lefelé, és válassza az **Alaphelyzet** gombot, majd a felugró panelen válassza ismét az **Alaphelyzet** gombot.</span><span class="sxs-lookup"><span data-stu-id="ffab8-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="ffab8-115">**2. lépés: A Microsoft Store gyorsítótárának kiürítése**</span><span class="sxs-lookup"><span data-stu-id="ffab8-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="ffab8-116">Nyomja le a Windows billentyűt + az R billentyűt a Futtatás párbeszédpanel megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="ffab8-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="ffab8-117">Írja be a wsreset.exe parancsot, és válassza az **OK** gombot.</span><span class="sxs-lookup"><span data-stu-id="ffab8-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="ffab8-118">Ekkor megnyílik egy üres parancssori ablak.</span><span class="sxs-lookup"><span data-stu-id="ffab8-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="ffab8-119">Körülbelül 10 másodperc elteltével az ablak bezárul, és automatikusan megnyílik a Store.</span><span class="sxs-lookup"><span data-stu-id="ffab8-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="ffab8-120">**3. lépés: A Windows Update alaphelyzetbe állítása**</span><span class="sxs-lookup"><span data-stu-id="ffab8-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="ffab8-121">Válassza a **Start** > **Gépház** > **Frissítés és biztonság** > **Hibaelhárítás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ffab8-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="ffab8-122">Görgessen lefelé, és jelölje ki a lista **Windows Update** elemét, majd válassza **A hibaelhárító futtatása** gombot.</span><span class="sxs-lookup"><span data-stu-id="ffab8-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="ffab8-123">Indítsa újra a számítógépet, és ellenőrizze, hogy továbbra is tapasztalja-e a problémát.</span><span class="sxs-lookup"><span data-stu-id="ffab8-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

