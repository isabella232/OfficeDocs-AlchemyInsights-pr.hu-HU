---
title: Az Android-eszközök regisztrálásával kapcsolatos hibák elhárítása a Microsoft Intune
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008080"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Az Android-eszközök regisztrálásával kapcsolatos hibák elhárítása a Microsoft Intune

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori probléma és megoldási lépés:
  
 **Az eszköz nincs titkosított hiba a Céges portál:** Az Android újabb verziói, különösen a 7.0-s verziótól kezdve, indítókódot igényelnek az eszköz teljes titkosításakor. Gyakori megoldás az indítási PIN-kód engedélyezése vagy az eszköz teljes titkosítása. További [információért tekintse](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) át ezt a dokumentumot.
  
 **Az eszközök nem jelennek meg az Intune-szolgáltatásban,** vagy hibásan jelennek meg az Intune felügyeleti konzolján: Egyes Samsung 4.4-es és 5.5-ös eszközök nem biztos, hogy bevetik a szolgáltatást. A problémának három lehetséges megoldása van:
  
1. Nyissa meg manuálisan Intune Céges portál appot, amely automatikusan elindítja az eszköz szinkronizálását.

2. Frissítse az eszközt Android 6.0-s vagy újabb verzióra.

3. Tiltsa le a Samsung Smart Manager számára a Intune Céges portál. A [dokumentumban további](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) részleteket talál ezekről a problémákról és megoldásukról.

 **Érvénytelen felhasználói licenctípus vagy** Nem felismerhető felhasználónév **hibaüzenet:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni. A licencek hozzárendeléshez tekintse át az alábbi dokumentumokat: Office Felügyeleti központ vagy az Azure Portal webhelyen.
  
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.

2. Ebben [a dokumentumban](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) áttekintheti azokat a gyakori hibákat, amelyek meggátolják a regisztrációt és a megoldást az egyes hibákra.

3. [Megtudhatja, hogy miként regisztrálható Android-eszközök a Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
