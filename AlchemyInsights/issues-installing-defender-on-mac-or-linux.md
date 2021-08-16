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
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013246"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémák a Microsoft Defender telepítésével Macen vagy Linuxon

**Mac**

- A Mac Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények. További információ: A [Microsoft Defender ATP telepítése Macre](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Ellenőrizze a fájlban található információkat: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- A Linuxhoz való Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények. További információt Az [MDATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)telepítése Linuxhoz . 
- Ha ellenőrizni, hogy fut-e az MDATP szolgáltatás, tekintse át a Nem sikerült [a telepítés.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Ha nem fut a szolgáltatás, a hibaelhárításhoz és a problémák megoldásához tekintse meg a Hibaelhárítási lépések, ha az [mdatp](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)szolgáltatás nem fut.
- A termék állapotát ellenőrző ügyfélkonfiguráció ellenőrzéséhez, valamint az EICAR szövegfájlon való észlelési teszt futtatásához lásd: [Ügyfélkonfiguráció.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Megjegyzés** A hozzáféréssel kapcsolatos tevékenységek támogatott fájlrendszereinek listáját a Linuxhoz használható [Microsoft Defender ATP webhelyén láthatja.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)