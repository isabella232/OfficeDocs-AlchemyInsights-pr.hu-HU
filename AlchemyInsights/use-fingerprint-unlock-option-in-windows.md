---
title: Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796679"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="e4839-102">Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="e4839-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="e4839-103">**Windows Hello ujjlenyomat engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="e4839-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="e4839-104">Ha ujjlenyomatával is fel szeretne oldani a Windows 10 zárolását, be kell állítania a Windows Hello-ujjlenyomatot úgy, hogy hozzáadja (a Windows megtanulja felismerni) legalább egy ujját.</span><span class="sxs-lookup"><span data-stu-id="e4839-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="e4839-105">Válassza **a Beállítások > Fiókok > Bejelentkezési** lehetőségek lehetőséget (vagy kattintson [ide).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="e4839-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e4839-106">Az elérhető bejelentkezési lehetőségek listája megjelenik.</span><span class="sxs-lookup"><span data-stu-id="e4839-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="e4839-107">Például:</span><span class="sxs-lookup"><span data-stu-id="e4839-107">For example:</span></span>

    ![Bejelentkezési lehetőségek.](media/sign-in-options.png)

2. <span data-ttu-id="e4839-109">Kattintson vagy koppintson a **Windows Hello Ujjlenyomat elemre,** majd a **Beállítás elemre.**</span><span class="sxs-lookup"><span data-stu-id="e4839-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="e4839-110">A Windows Hello beállítási ablakában kattintson az Első **lépések elemre.**</span><span class="sxs-lookup"><span data-stu-id="e4839-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="e4839-111">Az ujjlenyomat-érzékelő aktiválódik, és a rendszer megkéri, hogy helyezze az ujját az érzékelőre:</span><span class="sxs-lookup"><span data-stu-id="e4839-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Ujjlenyomat-érzékelő.](media/fingerprint-sensor.png)

3. <span data-ttu-id="e4839-113">Kövesse az utasításokat, amely arra fogja kérni, hogy többször olvassa be az ujját.</span><span class="sxs-lookup"><span data-stu-id="e4839-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="e4839-114">Ha ezzel végzett, további ujjakat is adhat hozzá, amelyekre a bejelentkezéshez szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="e4839-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="e4839-115">Amikor legközelebb bejelentkezik a Windows 10-be, az ujjlenyomatával is ezt is meg tudja tenni.</span><span class="sxs-lookup"><span data-stu-id="e4839-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="e4839-116">**A Windows Hello ujjlenyomat-olvasója nem érhető el bejelentkezési lehetőségként**</span><span class="sxs-lookup"><span data-stu-id="e4839-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="e4839-117">Ha a Bejelentkezési lehetőségek között nem látható a Windows Hello ujjlenyomat-olvasó, az azt jelenti, hogy a Windows nem tud a pc-hez csatlakoztatott ujjlenyomat-olvasóról vagy szkennerről, vagy hogy egy rendszer házirend akadályozza a használatát (ha például a **pc-t** a munkahelye kezeli).</span><span class="sxs-lookup"><span data-stu-id="e4839-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="e4839-118">Hibaelhárítás:</span><span class="sxs-lookup"><span data-stu-id="e4839-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="e4839-119">Válassza a **Start gombot** a tálcán, és keresse meg az **Eszközkezelőt.**</span><span class="sxs-lookup"><span data-stu-id="e4839-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="e4839-120">Kattintással vagy koppintással nyissa meg az **Eszközkezelőt.**</span><span class="sxs-lookup"><span data-stu-id="e4839-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="e4839-121">Az Eszközkezelőben bontsa ki a biometrikus eszközöket a sávnyílra kattintva.</span><span class="sxs-lookup"><span data-stu-id="e4839-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrikus eszközök.](media/biometric-devices.png)

4. <span data-ttu-id="e4839-123">Az ujjlenyomat-olvasónak biometrikus eszközként, például a Synaptics WBDI scannerben kell lennie:</span><span class="sxs-lookup"><span data-stu-id="e4839-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrikus eszközök.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="e4839-125">Ha az ujjlenyomat-olvasó nem látható, és a képolvasó integrálva van a PC-be, akkor a számítógép gyártójának webhelyére kell visszalaposodni.</span><span class="sxs-lookup"><span data-stu-id="e4839-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="e4839-126">A pc-modell technikai támogatási szakaszában keressen egy Windows 10-es illesztőprogramot, és keressen egy telepíthető képolvasót.</span><span class="sxs-lookup"><span data-stu-id="e4839-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="e4839-127">Ha a képolvasó nem található meg a PC-n (USB-n keresztül csatlakoztatva), keresse fel a képolvasó gyártójának webhelyét, és keresse meg és telepítse a windows 10-es eszközillesztő szoftverét a használt képolvasóhoz.</span><span class="sxs-lookup"><span data-stu-id="e4839-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
