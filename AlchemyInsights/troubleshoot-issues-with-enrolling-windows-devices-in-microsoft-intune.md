---
title: A Windows-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658880"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>A Windows-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori hibaüzenet és megoldási lépés:
  
 **A szoftver nem telepíthető, 0x80cf4017:** Lejárt a fiókja tanúsítványa. Töltse le újra a PC-kliens szoftvercsomagot az Intune felügyeleti konzolon. További információért olvassa el ezt a dokumentációt.
  
 **Hibakód 0x801c0003:** A hiba az alábbi esetekben fordulhat elő:
  
-  A felhasználó több olyan eszközt regisztrált, mint az eszköz korlátja. Tekintse át ezeket a dokumentumokat az [eszközök eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszköz korlátozásának módosításához](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "A felhasználók az Azure AD-hoz csatlakozhatnak eszközökhöz" beállítás értéke "nincs". Adja meg az összeset vagy válassza a felhasználók elemet. További információért olvassa el [ezt a dokumentációt](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Az eszközt már regisztrálta egy másik felhasználó. Ha ez a helyzet, távolítsa el az eszközt az Azure Intune konzolból, vagy manuálisan távolítsa el az eszközt, és próbálkozzon újra.

-  Az eszköz a Windows 10 Home. Csak a Windows 10 Pro, az oktatási és a vállalati SKU-hoz csatlakozhat az Azure Active Directoryhoz.

További források a probléma megoldásához:
  
-  Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat. További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .

-  Tekintse át ezeket a dokumentumokat a tanúsítványigénylést és az állásfoglalásokat akadályozó gyakori hibák listáját: [hibaelhárítási útmutató](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és [Hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Megtudhatja, hogy miként regisztrálhat Windows-eszközöket a Microsoft Intune-ban](https://docs.microsoft.com/intune/windows-enroll).
