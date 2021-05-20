---
title: Kivételek konfigurálása Microsoft Defender ATP vizsgálathoz
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543687"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="711ec-102">Kivételek konfigurálása Microsoft Defender ATP vizsgálathoz</span><span class="sxs-lookup"><span data-stu-id="711ec-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="711ec-103">Általában kizárhat bizonyos fájlkiterjesztéseket és mappahelyeket a Microsoft Defender ATP keresésekből.</span><span class="sxs-lookup"><span data-stu-id="711ec-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="711ec-104">Bizonyos folyamatok által megnyitott fájlok kivételét is konfigurálhatja.</span><span class="sxs-lookup"><span data-stu-id="711ec-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="711ec-105">További információ: Kivételek [](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) beállítása és érvényesítése fájlkiterjesztés és mappahely alapján és Kivételek konfigurálása a folyamatok által megnyitott [fájlokhoz.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="711ec-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="711ec-106">A kivételek beállítását a **Windows Server 2016 2019-es és 2019-es** Microsoft Defender víruskereső konfigurálja a [Windows kiszolgálón.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="711ec-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="711ec-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="711ec-107">**Mac**</span></span>

<span data-ttu-id="711ec-108">A támogatott kivételtípusokról és a Kivételek listájának konfigurálásával kapcsolatos részletekért lásd: Támogatott kivételtípusok és A kivételek [listájának konfigurálása.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions) [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="711ec-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="711ec-109">**Megjegyzés** A kivétellistákat az EICAR tesztfájl használatával is érvényesítheti.</span><span class="sxs-lookup"><span data-stu-id="711ec-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="711ec-110">További információt a Kivételek ellenőrzése [az EICAR tesztfájllal .](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="711ec-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="711ec-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="711ec-111">**Linux**</span></span>

<span data-ttu-id="711ec-112">A támogatott kivételtípusokról és a Linux kivételek listájának [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) konfigurálásával kapcsolatos részletekért lásd: Támogatott kivételtípusok és Kivételek konfigurálása és [Microsoft Defender ATP Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)rendszeren.</span><span class="sxs-lookup"><span data-stu-id="711ec-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="711ec-113">**Megjegyzés** A kivétellistákat az EICAR tesztfájl használatával is érvényesítheti.</span><span class="sxs-lookup"><span data-stu-id="711ec-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="711ec-114">További információt a Kivételek ellenőrzése [az EICAR tesztfájllal .](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="711ec-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 