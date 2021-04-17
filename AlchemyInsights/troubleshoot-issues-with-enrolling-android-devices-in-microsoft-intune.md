---
title: Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830944"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori probléma és megoldási lépés:
  
 **Az eszköz nincs titkosítva hibaüzenet a vállalati portálon:** Az Android újabb verziói, különösen a 7.0-s verziótól kezdve, indítókódot igényelnek az eszköz teljes titkosításakor. Gyakori megoldás az indítási PIN-kód engedélyezése vagy az eszköz teljes titkosítása. További [információért tekintse](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) át ezt a dokumentumot.
  
 **Az eszközök nem jelennek meg az Intune-szolgáltatásban,** vagy hibásan jelennek meg az Intune felügyeleti konzolján: Egyes Samsung 4.4-es és 5.5-ös eszközök nem biztos, hogy bevetik a szolgáltatást. A problémának három lehetséges megoldása van:
  
1. Nyissa meg manuálisan az Intune Céges portál appot, amely automatikusan elindítja az eszközszinkronizálást.

2. Frissítse az eszközt Android 6.0-s vagy újabb verzióra.

3. Tiltsa le a Samsung Smart Manager számára az Intune vállalati portál felügyeletét. A [dokumentumban további](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) részleteket talál ezekről a problémákról és megoldásukról.

 **Érvénytelen felhasználói licenctípus vagy** Nem felismerhető felhasználónév **hibaüzenet:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni. A következő dokumentumok alapján rendeljen licencet: Office Felügyeleti központ vagy Azure Portal.
  
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.

2. Ebben [a dokumentumban](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) áttekintheti azokat a gyakori hibákat, amelyek meggátolják a regisztrációt és a megoldást az egyes hibákra.

3. [Megtudhatja, hogy miként regisztrálható Android-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/android-enroll)
