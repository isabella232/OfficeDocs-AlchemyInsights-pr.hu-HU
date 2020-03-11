---
title: Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588318"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="a299c-102">Ujjlenyomat-feloldási lehetőség használata a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="a299c-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="a299c-103">**A Windows Hello ujjlenyomatának engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="a299c-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="a299c-104">A Windows 10 ujjlenyomatával történő feloldásához legalább egy ujjhozzáadásával (a Windows megtanulásával) be kell állítania a Windows Hello Fingerprint alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="a299c-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="a299c-105">Nyissa meg a **Beállítások > fiókok > bejelentkezési beállításokat** (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="a299c-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="a299c-106">Az elérhető bejelentkezési lehetőségek megjelennek a listában.</span><span class="sxs-lookup"><span data-stu-id="a299c-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="a299c-107">Például:</span><span class="sxs-lookup"><span data-stu-id="a299c-107">For example:</span></span>

    ![Bejelentkezési beállítások.](media/sign-in-options.png)

2. <span data-ttu-id="a299c-109">Kattintson vagy koppintson a **Windows Hello Fingerprint**elemre, majd a **Beállítás**gombra.</span><span class="sxs-lookup"><span data-stu-id="a299c-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="a299c-110">A Windows Hello beállítási ablakában kattintson az **Első lépések**gombra.</span><span class="sxs-lookup"><span data-stu-id="a299c-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="a299c-111">Az ujjlenyomat-érzékelő aktiválódik, és meg kell kérnie, hogy helyezze az ujját az érzékelőre:</span><span class="sxs-lookup"><span data-stu-id="a299c-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Ujjlenyomat-érzékelő.](media/fingerprint-sensor.png)

3. <span data-ttu-id="a299c-113">Kövesse az utasításokat, amelyek arra kérik, hogy többször is átkukkoljuk az ujját.</span><span class="sxs-lookup"><span data-stu-id="a299c-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="a299c-114">Ha ennek vége, lehetősége van arra, hogy további ujjakat adjon hozzá, amelyeket érdemes lehet használni a bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="a299c-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="a299c-115">Amikor legközelebb bejelentkezik a Windows 10-be, lehetősége van arra, hogy ujjlenyomatát használja ehhez.</span><span class="sxs-lookup"><span data-stu-id="a299c-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="a299c-116">**A Windows Hello ujjlenyomat nem érhető el bejelentkezési lehetőségként**</span><span class="sxs-lookup"><span data-stu-id="a299c-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="a299c-117">Ha a Windows Hello Ujjlenyomat nem jelenik meg lehetőségként a **Bejelentkezési beállításokban,** az azt jelenti, hogy a Windows nem tud a számítógéphez csatlakoztatott ujjlenyomat-olvasóról/lapolvasóról, vagy hogy a rendszerházirend megakadályozza annak használatát (ha például a számítógépet a munkahelye kezeli).</span><span class="sxs-lookup"><span data-stu-id="a299c-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="a299c-118">Hibaelhárítás:</span><span class="sxs-lookup"><span data-stu-id="a299c-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="a299c-119">Kattintson a **Tálca Start** gombjára, és keressen az **Eszközkezelő**kifejezésre.</span><span class="sxs-lookup"><span data-stu-id="a299c-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="a299c-120">Kattintson vagy koppintson az **Eszközkezelő**megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="a299c-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="a299c-121">Az Eszközkezelőben bontsa ki a Biometriai eszközöket a sávnyílra kattintva.</span><span class="sxs-lookup"><span data-stu-id="a299c-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrikus eszközök.](media/biometric-devices.png)

4. <span data-ttu-id="a299c-123">Az ujjlenyomat-szkennert biometrikus eszközként kell felsorolni, például a Synaptics WBDI szkennerként:</span><span class="sxs-lookup"><span data-stu-id="a299c-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrikus eszközök.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="a299c-125">Ha az ujjlenyomat-olvasó nem jelenik meg, és a lapolvasó be van építve a számítógépbe, keresse fel a számítógép gyártójának webhelyét.</span><span class="sxs-lookup"><span data-stu-id="a299c-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="a299c-126">A számítógép-modell technikai támogatási részében keressen egy Telepíthető képolvasó windows 10-illesztőprogramját.</span><span class="sxs-lookup"><span data-stu-id="a299c-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="a299c-127">Ha a lapolvasó elkülönül a számítógéptől (USB-n keresztül csatlakoztatva), keresse meg és telepítse a Windows 10 eszközillesztő szoftverét a képolvasó modellhez.</span><span class="sxs-lookup"><span data-stu-id="a299c-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
