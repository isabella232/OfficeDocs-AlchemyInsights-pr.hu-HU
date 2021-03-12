---
title: A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708892"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori hibaüzenet és megoldási lépés:
  
 **A szoftver nem telepíthető, és 0x80cf4017:** A fiók tanúsítványa lejárt. Töltse le újra a PC-ügyfél szoftvercsomagot az Intune Felügyeleti konzolon. További információt ebben a dokumentációban talál.
  
 **Hibakód 0x801c0003:** A hiba az alábbi esetekben fordulhat elő:
  
-  A felhasználó több eszközt regisztrált, mint az eszközkorlát. Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) vagy [módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  A "Felhasználók csatlakozhatnak az Azure AD-hez" beállítás "nincs" beállításra van állítva. Állítsa be az összes felhasználót, vagy jelöljön ki felhasználókat. További [információt ebben](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) a dokumentációban talál.

-  Az eszközt már regisztrálta egy másik felhasználó. Ebben az esetben távolítsa el az eszközt az Azure Intune konzolból, vagy manuálisan törölje az eszköz igénylését, mielőtt újra próbálkozik.

-  Az eszköz a Windows 10 Home. Az Azure Active Directoryhoz csak Windows 10 Pro, Oktatási és Nagyvállalati verziós SKUs csatlakozhat.

További források a probléma megoldásához:
  
-  Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és megoldhatja a gyakori regisztrációs hibákat. További [részletekért tekintse](https://docs.microsoft.com/intune/help-desk-operators) át ezt a dokumentumot.

-  Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, [](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) amelyek meggátolják a regisztrációt és az egyes problémák megoldását: hibaelhárítási útmutató és [hibaelhárítási dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Megtudhatja, hogy miként regisztrálja a Windows-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/windows-enroll)
