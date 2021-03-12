---
title: A Microsoft Defender Macen vagy Linuxon való telepítésével kapcsolatos problémák
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
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713836"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="7cc51-102">A Microsoft Defender Macen vagy Linuxon való telepítésével kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="7cc51-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="7cc51-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="7cc51-103">**Mac**</span></span>

- <span data-ttu-id="7cc51-104">A Mac Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények.</span><span class="sxs-lookup"><span data-stu-id="7cc51-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="7cc51-105">További információ: [A Microsoft Defender ATP telepítése Machez.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="7cc51-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="7cc51-106">Tekintse át a fájlban található információkat: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="7cc51-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="7cc51-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="7cc51-107">**Linux**</span></span>

- <span data-ttu-id="7cc51-108">A Linuxhoz telepített Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények.</span><span class="sxs-lookup"><span data-stu-id="7cc51-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="7cc51-109">További információ: [A Microsoft Defender ATP telepítése Linuxhoz.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="7cc51-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="7cc51-110">Az MDATP szolgáltatás futásának ellenőrzéséhez lásd: [Telepítés sikertelen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="7cc51-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="7cc51-111">Ha a szolgáltatás nem fut, a hibaelhárítási lépéseket követve elháríthatja, ha az [mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)szolgáltatás nem fut.</span><span class="sxs-lookup"><span data-stu-id="7cc51-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="7cc51-112">A termék állapotát ellenőrző ügyfélkonfiguráció ellenőrzéséhez, valamint az EICAR szövegfájlon való észlelési teszt futtatásához lásd: Ügyfél [konfigurációja.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="7cc51-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="7cc51-113">**Megjegyzés** A hozzáféréssel kapcsolatos tevékenységek támogatott fájlrendszereinek listáját a Linuxhoz használható [Microsoft Defender ATP szolgáltatásban tudja megnézni.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="7cc51-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>