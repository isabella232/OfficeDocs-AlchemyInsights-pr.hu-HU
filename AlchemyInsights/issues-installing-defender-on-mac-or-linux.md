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
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémák a Microsoft Defender telepítésével Macen vagy Linuxon

**Mac**

- A Mac Microsoft Defender ATP telepítése előtt győződjön meg arról, hogy teljesülnek a rendszerkövetelmények. További információ: A Mac Microsoft Defender ATP [telepítése.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Ellenőrizze a fájlban található információkat: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Győződjön meg arról, hogy a rendszerkövetelmények megfelelnek a Linux Microsoft Defender ATP telepítése előtt. További információért lásd: A [Linux MDATP telepítése.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Ha ellenőrizni, hogy MDATP szolgáltatás fut-e, tekintse át a Nem sikerült [a telepítés.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Ha nem fut a szolgáltatás, a hibaelhárításhoz és a problémák megoldásához tekintse meg a Hibaelhárítási lépések, ha az [mdatp](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)szolgáltatás nem fut.
- A termék állapotát ellenőrző ügyfélkonfiguráció ellenőrzéséhez, valamint az EICAR szövegfájlon való észlelési teszt futtatásához lásd: [Ügyfélkonfiguráció.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Megjegyzés** A hozzáférés-alapú tevékenységek támogatott fájlrendszereinek listáját A Linux rendszer Microsoft Defender ATP [sorolja fel.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)