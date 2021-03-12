---
title: Kivételek konfigurálása a Microsoft Defender ATP-vizsgálathoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713896"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="bee52-102">Kivételek konfigurálása a Microsoft Defender ATP-vizsgálathoz</span><span class="sxs-lookup"><span data-stu-id="bee52-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="bee52-103">Általában kizárhat bizonyos fájlkiterjesztéseket és mappahelyeket a Microsoft Defender ATP-vizsgálatból.</span><span class="sxs-lookup"><span data-stu-id="bee52-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="bee52-104">Bizonyos folyamatok által megnyitott fájlok kivételét is beállíthatja.</span><span class="sxs-lookup"><span data-stu-id="bee52-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="bee52-105">További információt a [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) kivételek konfigurálása és érvényesítése a fájlkiterjesztés és a mappa helye, valamint a folyamatok által megnyitott fájlok kivételének [konfigurálása alapján.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="bee52-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="bee52-106">A **kivételek Windows Server 2016-ra és 2019-re** való konfigurálásról a Microsoft Defender víruskereső kizárásának konfigurálása Windows Server [rendszeren.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="bee52-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="bee52-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="bee52-107">**Mac**</span></span>

<span data-ttu-id="bee52-108">A támogatott kivételtípusokról és a Mac kivételek listájának [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) konfigurálásáról a Támogatott kivételtípusok és a Kivételek listájának konfigurálása a [részletekben olvashat.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="bee52-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="bee52-109">**Megjegyzés** A kivétellistákat az EICAR tesztfájl használatával is érvényesítheti.</span><span class="sxs-lookup"><span data-stu-id="bee52-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="bee52-110">További információt a kivételek ellenőrzése az [EICAR tesztfájllal.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="bee52-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="bee52-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="bee52-111">**Linux**</span></span>

<span data-ttu-id="bee52-112">A támogatott kivételtípusokról és a linuxos kivételek listájának konfigurálásáról további információt a Támogatott kivételtípusok és a Kivételek konfigurálása és érvényesítése a Linuxhoz használható [Microsoft Defender ATP szolgáltatásban.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions) [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="bee52-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="bee52-113">**Megjegyzés** A kivétellistákat az EICAR tesztfájl használatával is érvényesítheti.</span><span class="sxs-lookup"><span data-stu-id="bee52-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="bee52-114">További információt a kivételek ellenőrzése az [EICAR tesztfájllal.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="bee52-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 