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
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>A Microsoft Defender Macen vagy Linuxon való telepítésével kapcsolatos problémák

**Mac**

- A Mac Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények. További információ: [A Microsoft Defender ATP telepítése Machez.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Tekintse át a fájlban található információkat: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- A Linuxhoz telepített Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények. További információ: [A Microsoft Defender ATP telepítése Linuxhoz.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Az MDATP szolgáltatás futásának ellenőrzéséhez lásd: [Telepítés sikertelen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Ha a szolgáltatás nem fut, a hibaelhárítási lépéseket követve elháríthatja, ha az [mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)szolgáltatás nem fut.
- A termék állapotát ellenőrző ügyfélkonfiguráció ellenőrzéséhez, valamint az EICAR szövegfájlon való észlelési teszt futtatásához lásd: Ügyfél [konfigurációja.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Megjegyzés** A hozzáféréssel kapcsolatos tevékenységek támogatott fájlrendszereinek listáját a Linuxhoz használható [Microsoft Defender ATP szolgáltatásban tudja megnézni.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)