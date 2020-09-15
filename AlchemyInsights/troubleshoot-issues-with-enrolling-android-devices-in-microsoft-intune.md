---
title: Az Android-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689956"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Az Android-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Néhány gyakori probléma és megoldási lépés:
  
 **A vállalati portál eszköz nem titkosított hibája:** Az Android újabb verzióihoz, különösen a v 7.0-s verziójához, indítási hitelesítő kód szükséges ahhoz, hogy az eszköz teljes mértékben titkosítva legyen. A gyakori megoldásokkal engedélyezheti az indítási PIN-kódot, vagy teljes mértékben titkosíthatja az eszközt. További információt a [dokumentum](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) véleményezése című témakörben olvashat.
  
 **Az Intune felügyeleti konzoljában az eszközök nem jelennek meg a Intune szolgáltatással, vagy a "nem egészséges" megjelenítéssel:** Előfordulhat, hogy egyes Samsung 4,4-és 5,5-eszközök nem kerülnek be a szolgáltatásba. Ebből a problémából 3 lehetséges megoldás áll rendelkezésre:
  
1. Nyissa meg manuálisan az Intune vállalati portál alkalmazást, amely automatikusan elindítja az eszköz szinkronizálását.

2. Frissítse az eszközt Android 6,0-es vagy újabb verzióra.

3. Tiltsa le a Samsung Smart Managert az Intune vállalati portál kezelésének letiltásával. Tekintse át a következő témakört, és olvassa el a fenti problémákat és állásfoglalásokat ismertető [dokumentumot](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) .

 A **felhasználói licenc típusa érvénytelen** vagy a **Felhasználónév nem ismerhető fel hiba:** a felhasználónak Intune vagy EMS licenccel kell rendelkeznie. Ezekkel a dokumentumokkal az Office felügyeleti központból vagy az Azure portálról rendelhet licencet:
  
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat. További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .

2. Tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) azoknak a gyakori hibáknak a listáját, amelyekkel megelőzheti a beiratkozási és a felbontást.

3. [Megtudhatja, hogy miként regisztrálhat Android-eszközöket a Microsoft Intune-ban](https://docs.microsoft.com/intune/android-enroll).
