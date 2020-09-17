---
title: Az ujjlenyomat feloldása funkció használata Windows 10 rendszerben
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795246"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="44433-102">Az ujjlenyomat feloldása funkció használata Windows 10 rendszerben</span><span class="sxs-lookup"><span data-stu-id="44433-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="44433-103">**A Windows Hello ujjlenyomat engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="44433-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="44433-104">Ha a Windows 10 rendszert az ujjlenyomatával szeretné feloldani, a Windows Hello ujjlenyomatot úgy kell beállítania, hogy hozzáadja a (Windows megismerése) gombot legalább egy ujjal.</span><span class="sxs-lookup"><span data-stu-id="44433-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="44433-105">Lépjen a **beállítások >-fiókok > bejelentkezési beállítások** elemre (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="44433-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="44433-106">A rendelkezésre álló bejelentkezési beállítások megjelennek.</span><span class="sxs-lookup"><span data-stu-id="44433-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="44433-107">Például:</span><span class="sxs-lookup"><span data-stu-id="44433-107">For example:</span></span>

    ![Bejelentkezési lehetőségek](media/sign-in-options.png)

2. <span data-ttu-id="44433-109">Kattintson vagy koppintson a **Windows Hello ujjlenyomat**elemre, majd a **beállítás**gombra.</span><span class="sxs-lookup"><span data-stu-id="44433-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="44433-110">A Windows Hello Setup ablakában kattintson az első **lépések**elemre.</span><span class="sxs-lookup"><span data-stu-id="44433-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="44433-111">Az ujjlenyomat-érzékelő aktívvá válik, és a rendszer arra kéri, hogy helyezze az ujját az érzékelőre:</span><span class="sxs-lookup"><span data-stu-id="44433-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Ujjlenyomat-érzékelő](media/fingerprint-sensor.png)

3. <span data-ttu-id="44433-113">Kövesse az utasításokat, amelyek arra kérik, hogy rendszeresen ellenőrizze az ujját.</span><span class="sxs-lookup"><span data-stu-id="44433-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="44433-114">Ha végzett, akkor lehetősége van a bejelentkezéshez használni kívánt egyéb ujjak hozzáadására.</span><span class="sxs-lookup"><span data-stu-id="44433-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="44433-115">A következő alkalommal, amikor bejelentkezik a Windows 10-be, megadhatja, hogy hogyan használhatja az ujjlenyomatát.</span><span class="sxs-lookup"><span data-stu-id="44433-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="44433-116">**A Windows Hello ujjlenyomata nem érhető el bejelentkezési beállításként**</span><span class="sxs-lookup"><span data-stu-id="44433-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="44433-117">Ha a Windows Hello ujjlenyomat nem jelenik meg a **bejelentkezési beállítások**között, az azt jelenti, hogy a Windows nem ismeri a számítógéphez csatlakoztatott ujjlenyomat-olvasót/szkennert, vagy hogy a Rendszerházirend megakadályozza annak használatát (Ha például a számítógépe a munkahelye kezeli).</span><span class="sxs-lookup"><span data-stu-id="44433-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="44433-118">Hibaelhárítás:</span><span class="sxs-lookup"><span data-stu-id="44433-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="44433-119">Válassza a tálcán a **Start** gombot, és keresse meg az **Eszközkezelőt**.</span><span class="sxs-lookup"><span data-stu-id="44433-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="44433-120">Kattintson vagy koppintson az **Eszközkezelő**megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="44433-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="44433-121">Az Eszközkezelőben a saját Chevron elemre kattintva bontsa ki a biometrikus eszközök elemet.</span><span class="sxs-lookup"><span data-stu-id="44433-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrikus eszközök.](media/biometric-devices.png)

4. <span data-ttu-id="44433-123">Az ujjlenyomat-szkennert biometrikus eszközként (például a Synaptics WBDI scanner) kell felsorolni:</span><span class="sxs-lookup"><span data-stu-id="44433-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrikus eszközök.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="44433-125">Ha az ujjlenyomat-szkennere nem látható, és a szkenner be van építve a SZÁMÍTÓGÉPére, lépjen a számítógép gyártójának webhelyére.</span><span class="sxs-lookup"><span data-stu-id="44433-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="44433-126">A PC-modell Technical Support (terméktámogatás) szakaszában keressen egy Windows 10-es illesztőprogramot a telepítendő képolvasóhoz.</span><span class="sxs-lookup"><span data-stu-id="44433-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="44433-127">Ha a szkenner el van választva a PC-ről (USB-n keresztül), nyissa meg a képolvasó gyártójának webhelyét, ahol megkeresheti és telepítheti a Windows 10-es eszközillesztő szoftvert a beolvasó modellhez.</span><span class="sxs-lookup"><span data-stu-id="44433-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
