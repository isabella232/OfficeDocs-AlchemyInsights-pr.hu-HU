---
title: Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709000"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori probléma és megoldási lépés:
  
 **Az eszköz nincs titkosítva hiba a céges portálon:** Az Android újabb verzióinak , különösen a 7.0-s verziótól kezdve, indítási pin-kódra van szükségük ahhoz, hogy az eszköz teljesen titkosított legyen. Gyakori megoldás az indítási pin-kód engedélyezése vagy az eszköz teljes titkosítása. További [információért tekintse](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) át ezt a dokumentumot.
  
 Az eszközök nem jelennek meg az Intune szolgáltatásban, vagy hibásan jelennek meg az **Intune felügyeleti konzolján:** Egyes Samsung 4.4-es és 5.5-ös eszközök nem biztos, hogy bevetik a szolgáltatást. A problémának három lehetséges megoldása van:
  
1. Nyissa meg manuálisan az Intune Vállalati portál alkalmazást, amely automatikusan elindítja az eszközszinkronizálást.

2. Frissítse az eszközt Android 6.0-s vagy újabb verzióra.

3. Tiltsa le a Samsung Smart Manager számára az Intune vállalati portál felügyeletét. A [problémaokkal](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) és megoldásokkal kapcsolatos további részletekért tekintse át ezt a dokumentumot.

 **Érvénytelen felhasználói licenctípus** vagy nem felismerhető felhasználónév **hiba:** A felhasználónak Intune- vagy EMS-licenccel kell rendelkezik. Tekintse át ezeket a dokumentumokat, és rendeljen licencet a következőn keresztül: Office Felügyeleti központ vagy Azure Portal.
  
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és megoldhatja a gyakori regisztrációs hibákat. További [részletekért tekintse](https://docs.microsoft.com/intune/help-desk-operators) át ezt a dokumentumot.

2. Ebben [a dokumentumban](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) áttekintheti azokat a gyakori hibákat, amelyek meggátolják a regisztrációt és az egyes problémák megoldását.

3. [Megtudhatja, hogy miként regisztrálható Android-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/android-enroll)
