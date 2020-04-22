---
title: Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759622"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori probléma és megoldási lépés:
  
 **Az eszköz nem titkosított hiba a céges portálon:** Az Android újabb verziói, különösen a 7.0-s verzióval kezdve, indítási jelkódot igényelnek annak érdekében, hogy az eszköz teljesen titkosítva legyen. A gyakori megoldások az indítópin engedélyezése vagy az eszköz teljes titkosítása. További információkért tekintse át ezt a [dokumentumot.](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)
  
 **Az eszközök nem jelentkeznek be az Intune szolgáltatással, vagy "Nem kifogástalan" állapotúként jelennek meg az Intune felügyeleti konzolján:** Előfordulhat, hogy egyes Samsung 4.4 és 5.5 eszközök nem jelentkeznek be a szolgáltatásba. A probléma 3 lehetséges megoldása lehetséges:
  
1. Manuálisan nyissa meg az Intune Céges portál alkalmazást, amely automatikusan elindítja az eszközszinkronizálást.

2. Frissítse az eszközt Android 6.0-s vagy újabb verzióra.

3. Tiltsa le a Samsung Smart Manager t az Intune vállalati portáljának kezelésében. Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) a további részletekért ezekről a kérdésekről és állásfoglalásokról.

 **Érvénytelen felhasználói licenctípus** vagy **nem felismert felhasználónév hiba:** A felhasználóhoz Intune- vagy EMS-licencet kell rendelni. Tekintse át ezeket a dokumentumokat, hogy licencet rendeljen az Office Felügyeleti központon vagy az Azure Portalon keresztül.
  
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat. Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért.

2. Tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és a megoldásokat.

3. [Megtudhatja, hogy miként regisztrálhat Android-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/android-enroll)
