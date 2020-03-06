---
title: Indítási beállítások a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409061"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="85c4d-102">Indítási beállítások a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="85c4d-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="85c4d-103">**Az indításkor automatikusan futó alkalmazások módosítása**</span><span class="sxs-lookup"><span data-stu-id="85c4d-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="85c4d-104">Nyissa meg a [Beállítások > alkalmazások > indításlehetőséget.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="85c4d-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="85c4d-105">Győződjön meg arról, hogy az indításkor futtatni kívánt alkalmazások **be**vannak kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="85c4d-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="85c4d-106">**Alkalmazás hozzáadása automatikus futtatáshoz indításkor**</span><span class="sxs-lookup"><span data-stu-id="85c4d-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="85c4d-107">Kattintson vagy koppintson a **Start** gombra, és keresse meg az indításkor futtatni kívánt alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="85c4d-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="85c4d-108">Kattintson a jobb gombbal az alkalmazásra, válassza az **Egyebek**, majd **a Fájlhely megnyitása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="85c4d-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="85c4d-109">Ezzel megnyitja azt a helyet, ahová az alkalmazás parancsikonját menti.</span><span class="sxs-lookup"><span data-stu-id="85c4d-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="85c4d-110">Ha nincs lehetőség a Fájl helyének megnyitása beállításra, az azt jelenti, hogy az alkalmazás nem futtatható indításkor.</span><span class="sxs-lookup"><span data-stu-id="85c4d-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="85c4d-111">Ha a fájl helye meg van nyitva, nyomja le a **Windows billentyű + R**billentyűkombinációt, írja be a **shell:startup**billentyűt, majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="85c4d-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="85c4d-112">Ekkor megnyílik az Indítópult mappa.</span><span class="sxs-lookup"><span data-stu-id="85c4d-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="85c4d-113">Másolja és illessze be az alkalmazásparancsikont a fájl helyéről az Indítóindító mappába.</span><span class="sxs-lookup"><span data-stu-id="85c4d-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="85c4d-114">**Speciális indítási beállítások (beleértve a csökkentett módot, az UEFI-beállításokat és a másik eszközről történő rendszerindítást)**</span><span class="sxs-lookup"><span data-stu-id="85c4d-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="85c4d-115">Mentse munkáját, és zárja be a megnyitott dokumentumokat, mivel ezek a lépések újraindítják a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="85c4d-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="85c4d-116">Nyissa meg a [Beállítások > Frissítés & Biztonsági > helyreállítás](ms-settings:recovery?activationSource=GetHelp)t.</span><span class="sxs-lookup"><span data-stu-id="85c4d-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="85c4d-117">A **Speciális indítás**csoportban kattintson az Újraindítás **gombra.**</span><span class="sxs-lookup"><span data-stu-id="85c4d-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="85c4d-118">Miután a számítógép újraindul a Választólehetőség képernyőre:</span><span class="sxs-lookup"><span data-stu-id="85c4d-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="85c4d-119">Ha usb-meghajtóról szeretne rendszerindítást szeretne, kattintson az **Eszköz használata**gombra.</span><span class="sxs-lookup"><span data-stu-id="85c4d-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="85c4d-120">Az UEFI-beállítások (más néven BIOS-beállítások) megadásához kattintson **a Speciális beállítások > az UEFI belső vezérlőprogram beállításai> hibaelhárítása gombra.**</span><span class="sxs-lookup"><span data-stu-id="85c4d-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="85c4d-121">A csökkentett mód megadásához vagy a speciális indítási beállítások módosításához kattintson a Speciális beállítások > > **indítási beállítások kal,** majd **az Újraindítás**gombra.</span><span class="sxs-lookup"><span data-stu-id="85c4d-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="85c4d-122">Előfordulhat, hogy meg kell adnia a [BitLocker helyreállítási kulcsot.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="85c4d-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="85c4d-123">A számítógép újraindítása után kattintson a használni kívánt indítási beállításra.</span><span class="sxs-lookup"><span data-stu-id="85c4d-123">After your PC restarts again, click the startup setting you want to use.</span></span>