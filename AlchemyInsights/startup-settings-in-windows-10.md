---
title: A Windows 10 indítási beállításai
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828154"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="70bdf-102">A Windows 10 indítási beállításai</span><span class="sxs-lookup"><span data-stu-id="70bdf-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="70bdf-103">**Annak módosítása, hogy mely alkalmazások futnak automatikusan indításkor**</span><span class="sxs-lookup"><span data-stu-id="70bdf-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="70bdf-104">Kattintson a [Beállítások > Alkalmazások > gombra.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="70bdf-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="70bdf-105">Győződjön meg arról, hogy az indításkor futtatni kívánt alkalmazások be vannak **kapcsolva.**</span><span class="sxs-lookup"><span data-stu-id="70bdf-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="70bdf-106">**Automatikusan elinduló alkalmazás hozzáadása**</span><span class="sxs-lookup"><span data-stu-id="70bdf-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="70bdf-107">Kattintson vagy **koppintson a Start gombra,** és keresse meg az indításkor futtatni kívánt alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="70bdf-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="70bdf-108">Kattintson a jobb gombbal az appra, kattintson az Egyéb **parancsra,** majd a Fájl **helyének megnyitása parancsra.**</span><span class="sxs-lookup"><span data-stu-id="70bdf-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="70bdf-109">Ezzel megnyitja azt a helyet, ahová az alkalmazás parancsikonja mentve van.</span><span class="sxs-lookup"><span data-stu-id="70bdf-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="70bdf-110">Ha nincs lehetőség a Fájl helyének megnyitása beállításra, az azt jelenti, hogy az alkalmazás nem tud elindulni.</span><span class="sxs-lookup"><span data-stu-id="70bdf-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="70bdf-111">Nyissa meg a fájl helyét, nyomja le a Windows billentyű **+ R** billentyűkombinációt, írja be a **shell:startup** parancsot, majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="70bdf-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="70bdf-112">Ezzel megnyitja az Indítópult mappát.</span><span class="sxs-lookup"><span data-stu-id="70bdf-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="70bdf-113">Másolja és illessze be az alkalmazás parancsikonját a fájl helyéről az Indítópult mappába.</span><span class="sxs-lookup"><span data-stu-id="70bdf-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="70bdf-114">**Speciális indítási beállítások (beleértve a csökkentett módot, az UEFI-beállításokat és a másik eszközről való indítást)**</span><span class="sxs-lookup"><span data-stu-id="70bdf-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="70bdf-115">Mentse a munkáját, és zárja be a megnyitott dokumentumokat, mivel ezek a lépések újraindítják a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="70bdf-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="70bdf-116">Kattintson a [Beállítások > Biztonsági & vagy > elemre.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="70bdf-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="70bdf-117">A **Speciális indítás alatt** kattintson az Újraindítás **gombra.**</span><span class="sxs-lookup"><span data-stu-id="70bdf-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="70bdf-118">A PC újraindítása után a Válasszon egy lehetőséget képernyőn:</span><span class="sxs-lookup"><span data-stu-id="70bdf-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="70bdf-119">Ha egy eszközről, például egy USB-meghajtóról szeretne indulni, kattintson **az Eszköz használata elemre.**</span><span class="sxs-lookup"><span data-stu-id="70bdf-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="70bdf-120">Az UEFI-beállítások (MÁS néven A. OKT.) beállításához kattintson az **UEFI** belső vezérlőprogram beállításai > Speciális beállítások > hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="70bdf-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="70bdf-121">A csökkentett mód beállításához vagy a speciális indítási beállítások módosításához kattintson a Speciális beállítások hibaelhárítása > indítási beállítások > **,** majd kattintson az Újraindítás **gombra.**</span><span class="sxs-lookup"><span data-stu-id="70bdf-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="70bdf-122">A rendszer megkérheti, hogy adja meg [a BitLocker helyreállítási kulcsot.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="70bdf-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="70bdf-123">A számítógép újraindítása után kattintson a használni kívánt indítási beállításra.</span><span class="sxs-lookup"><span data-stu-id="70bdf-123">After your PC restarts again, click the startup setting you want to use.</span></span>