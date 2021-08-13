---
title: A Windows eszköz regisztrálásával kapcsolatos Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981043"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>A Windows eszköz regisztrálásával kapcsolatos Microsoft Intune

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Gyakori hibaüzenetek és megoldási lépések:
  
 **A szoftvert nem lehet telepíteni, mert ez 0x80cf4017:** A fiók tanúsítványa lejárt. Töltse le újra a PC-ügyfélszoftver csomagját az Intune Felügyeleti konzolon. További információt ebben a dokumentációban talál.
  
 **Hibakód 0x801c0003:** A hiba az alábbi esetekben fordulhat elő:
  
-  A felhasználónak több eszköze van regisztrálva, mint az eszközkorlát. Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) [vagy módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  A "Felhasználók csatlakozhatnak az Azure AD-hez" beállítás "nincs" beállításra van állítva. Állítsa be az összes felhasználóra, vagy válassza ki a kívánt felhasználókat. További [információt ebben](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) a dokumentációban talál.

-  Az eszközt már regisztrálta egy másik felhasználó. Ha ez a helyzet, távolítsa el az eszközt az Azure Intune konzolból, vagy manuálisan törölje az eszköz igénylését, mielőtt újra próbálkozik.

-  Az eszköz Windows 10 Home. Csak Windows 10 Pro, az Oktatási és Nagyvállalati verziós verziók csatlakozhatnak a Azure Active Directory.

További források a probléma megoldásához:
  
-  Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.

-  Az alábbi dokumentumokban áttekintheti azoknak a gyakori hibáknak a listáját, amelyek meggátolják az regisztrációt és megoldást: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és a [Hibaelhárítási dokumentum](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Megtudhatja, hogy miként regisztrálja Windows eszközét a Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
