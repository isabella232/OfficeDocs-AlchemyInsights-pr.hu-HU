---
title: Problémák a Microsoft Defender telepítésével Macen vagy Linuxon
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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539682"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="8706f-102">Problémák a Microsoft Defender telepítésével Macen vagy Linuxon</span><span class="sxs-lookup"><span data-stu-id="8706f-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="8706f-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="8706f-103">**Mac**</span></span>

- <span data-ttu-id="8706f-104">A Mac Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények.</span><span class="sxs-lookup"><span data-stu-id="8706f-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="8706f-105">További információ: A Mac Microsoft Defender ATP [telepítése.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="8706f-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="8706f-106">Ellenőrizze a fájlban található információkat: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="8706f-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="8706f-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="8706f-107">**Linux**</span></span>

- <span data-ttu-id="8706f-108">Győződjön meg arról, hogy a rendszerkövetelmények megfelelnek a Linux Microsoft Defender ATP telepítése előtt.</span><span class="sxs-lookup"><span data-stu-id="8706f-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="8706f-109">További információért lásd: A [Linux MDATP telepítése.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="8706f-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="8706f-110">Ha ellenőrizni, hogy MDATP szolgáltatás fut-e, tekintse át a Nem sikerült [a telepítés.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="8706f-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="8706f-111">Ha nem fut a szolgáltatás, a hibaelhárításhoz és a problémák megoldásához tekintse meg a Hibaelhárítási lépések, ha az [mdatp](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)szolgáltatás nem fut.</span><span class="sxs-lookup"><span data-stu-id="8706f-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="8706f-112">A termék állapotát ellenőrző ügyfélkonfiguráció ellenőrzéséhez, valamint az EICAR szövegfájlon való észlelési teszt futtatásához lásd: [Ügyfélkonfiguráció.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="8706f-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="8706f-113">**Megjegyzés** A hozzáférés-alapú tevékenységek támogatott fájlrendszereinek listáját A Linux rendszer Microsoft Defender ATP [sorolja fel.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="8706f-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>