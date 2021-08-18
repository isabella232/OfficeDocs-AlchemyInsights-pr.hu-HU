---
title: A Microsoft Defender Mac vagy Linux rendszeren való telepítésével kapcsolatos problémák
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
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898610"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>A Microsoft Defender Mac vagy Linux rendszeren való telepítésével kapcsolatos problémák

**Mac**

- A Mac Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények. További információ: A [Microsoft Defender ATP telepítése Macre](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Ellenőrizze a fájlban található információkat: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- A Linuxhoz való Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények. További információt Az [MDATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)telepítése Linuxhoz . 
- Ha ellenőrizni, hogy fut-e az MDATP szolgáltatás, tekintse át a Nem sikerült [a telepítés.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Ha nem fut a szolgáltatás, a hibaelhárításhoz és a problémák megoldásához tekintse meg a Hibaelhárítási lépések, ha az [mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)szolgáltatás nem fut.
- A termék állapotát ellenőrző ügyfélkonfiguráció ellenőrzéséhez, valamint az EICAR szövegfájlon való észlelési teszt futtatásához lásd: [Ügyfélkonfiguráció.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Megjegyzés** A hozzáféréssel kapcsolatos tevékenységek támogatott fájlrendszereinek listáját a Linuxhoz használható [Microsoft Defender ATP webhelyén láthatja.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)