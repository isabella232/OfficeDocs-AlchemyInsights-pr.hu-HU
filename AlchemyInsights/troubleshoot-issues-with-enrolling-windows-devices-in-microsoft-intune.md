---
title: A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665834"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori hibaüzenet és megoldási lépés:
  
 **A szoftver nem telepíthető, 0x80cf4017:** A fióktanúsítvány lejárt. Töltse le újra a PC-ügyfél szoftvercsomagot az Intune felügyeleti konzolján. További információkért tekintse át ezt a dokumentációt.
  
 **0x801c0003 hibakód:** A hiba a következő esetekben fordulhat elő:
  
-  A felhasználó több eszközt regisztrált, mint az eszköz korlátját. Tekintse át ezeket a dokumentumokat [az eszköz eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszközkorlát módosításához.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "A felhasználók csatlakozhatnak az Azure AD-hez" beállítás "nincs" lesz. Állítsa be az összes, vagy válassza ki a felhasználókat. További információkért tekintse át ezt a [dokumentációt.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)

-  Az eszközt már regisztrálta egy másik felhasználó. Ebben az esetben távolítsa el az eszközt az Azure Intune konzolról, vagy manuálisan szüntesse meg az eszközt, mielőtt újra próbálkozna.

-  Az eszköz a Windows 10 Home. Csak a Windows 10 Pro, oktatási és nagyvállalati ska-k csatlakozhatnak az Azure Active Directoryhoz.

További források a probléma megoldásához:
  
-  Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat. Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért.

-  Tekintse át ezeket a dokumentumokat a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és az egyes megoldásokat: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és [hibaelhárítás idopont](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Megtudhatja, hogy miként regisztrálhat Windows-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/windows-enroll)
