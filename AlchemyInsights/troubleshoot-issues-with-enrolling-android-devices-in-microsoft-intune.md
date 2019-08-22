---
title: Android-eszköz a Microsoft Intune igénylése problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500073"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Android-eszköz a Microsoft Intune igénylése problémáinak elhárítása

Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése.
  
Néhány gyakori problémát, illetve lépéseket:
  
 **Eszköz nem titkosított hiba a vállalati portál:** Újabb verziói, Android, különösen v7.0, kezdve a rendszerindítási kódot győződjön meg arról, hogy az eszköz teljes mértékben titkosított van szükség. Közös megoldások indító PIN-kód engedélyezése, vagy az eszköz teljes mértékben titkosítja. További információt [a dokumentum](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) áttekintése.
  
 **Eszközök sikertelen, ellenőrizze a a Intune szolgáltatást, vagy "Unhealthy" a Intune felügyeleti konzolban jeleníti meg:** Néhány Samsung 4.4. és 5.5-ös eszközök nem ellenőrizheti az üzembe helyezés. Van 3 lehetséges megoldás a probléma:
  
1. Manuálisan nyissa meg a vállalati portál Intune app, amely automatikusan kezdeményez egy eszköz szinkronizálás.

2. Az eszköz az Android 6.0-s vagy újabb frissítés.

3. Samsung intelligens kezelő letiltása az Intune vállalati portál kezelése. [Ez a dokumentum](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) további részleteket a következő problémák és megoldások áttekintése.

 **Felhasználói licenc típusa érvénytelen** vagy **felhasználói neve ismeretlen hiba:** a felhasználónak kell egy Intune vagy EMS licencet kap. Tekintse át ezeket a dokumentumokat keresztül licenc hozzárendelése: Office Admin Center vagy Azure portal.
  
A probléma megoldásához további erőforrások:
  
1. [Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/intune/help-desk-operators) további részletekért tekintse át.

2. Tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listáját.

3. [Útmutató: Android-eszköz a Microsoft Intune igényelni](https://docs.microsoft.com/intune/android-enroll).
