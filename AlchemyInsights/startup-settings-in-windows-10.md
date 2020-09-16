---
title: Indítási beállítások a Windows 10 rendszerben
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751137"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="87690-102">Indítási beállítások a Windows 10 rendszerben</span><span class="sxs-lookup"><span data-stu-id="87690-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="87690-103">**A rendszerindítás során automatikusan futtatandó alkalmazások módosítása**</span><span class="sxs-lookup"><span data-stu-id="87690-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="87690-104">Nyissa meg a [beállítások > alkalmazásokat > indítás lehetőséget](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="87690-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="87690-105">Ellenőrizze, hogy **be van-e kapcsolva az**indításkor futtatni kívánt összes alkalmazás.</span><span class="sxs-lookup"><span data-stu-id="87690-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="87690-106">**Automatikusan futtatott alkalmazás felvétele indításkor**</span><span class="sxs-lookup"><span data-stu-id="87690-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="87690-107">Kattintson vagy koppintson a **Start** gombra, és keresse meg az indításkor futtatni kívánt alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="87690-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="87690-108">Kattintson a jobb gombbal az alkalmazásra, kattintson az **egyebek**, majd a **fájl helyének megnyitása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="87690-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="87690-109">Ezzel megnyitja azt a helyet, ahol az alkalmazás parancsikonja mentve van.</span><span class="sxs-lookup"><span data-stu-id="87690-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="87690-110">Ha a fájl helyének megnyitására nincs lehetőség, az azt jelenti, hogy az alkalmazás nem futtatható indításkor.</span><span class="sxs-lookup"><span data-stu-id="87690-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="87690-111">A fájl helyének megnyitásához nyomja le a **Windows billentyű + R**billentyűkombinációt, írja be a **Shell: Startup**parancsot, majd kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="87690-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="87690-112">Ekkor megnyílik az Indítópult mappa.</span><span class="sxs-lookup"><span data-stu-id="87690-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="87690-113">Másolja a vágólapra, majd illessze be a parancsikont az alkalmazásba a fájl helyéről az Indítópult mappájába.</span><span class="sxs-lookup"><span data-stu-id="87690-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="87690-114">**Speciális indítási beállítások (többek között a csökkentett mód, az UEFI-beállítások és egy másik eszközről való rendszerindítás)**</span><span class="sxs-lookup"><span data-stu-id="87690-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="87690-115">Mentse a munkáját, és zárjon be minden megnyitott dokumentumot, mert ezek a lépések a számítógép újraindítását követően jelentkeznek be.</span><span class="sxs-lookup"><span data-stu-id="87690-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="87690-116">Nyissa meg a [beállítások > a frissítés & biztonsági > helyreállítási](ms-settings:recovery?activationSource=GetHelp)lapját.</span><span class="sxs-lookup"><span data-stu-id="87690-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="87690-117">A **speciális indítás**csoportban kattintson az **Újraindítás most**elemre.</span><span class="sxs-lookup"><span data-stu-id="87690-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="87690-118">Miután a számítógép újraindult az Option (beállítások kiválasztása) képernyőre:</span><span class="sxs-lookup"><span data-stu-id="87690-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="87690-119">Ha USB-meghajtóról szeretne indítani egy eszközt, kattintson az **eszköz használata**elemre.</span><span class="sxs-lookup"><span data-stu-id="87690-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="87690-120">Az UEFI-beállítások (más néven BIOS-beállítás) megadásához kattintson a **> speciális beállítások hibaelhárítása > UEFI firmware beállításai**parancsra.</span><span class="sxs-lookup"><span data-stu-id="87690-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="87690-121">A csökkentett mód megadásához vagy a speciális indítási beállítások módosításához kattintson az **indítási beállítások > speciális beállítások elhárítása > indítási beállítások**gombra, majd az **Újraindítás**parancsra.</span><span class="sxs-lookup"><span data-stu-id="87690-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="87690-122">A rendszer kérheti a [BitLocker helyreállítási kulcs](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)megadását.</span><span class="sxs-lookup"><span data-stu-id="87690-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="87690-123">Miután a számítógép ismét újraindult, kattintson a használni kívánt indítási beállításra.</span><span class="sxs-lookup"><span data-stu-id="87690-123">After your PC restarts again, click the startup setting you want to use.</span></span>