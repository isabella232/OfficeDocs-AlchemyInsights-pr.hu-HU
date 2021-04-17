---
title: A Microsoft Intune-ban az Adatszolgáltató regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 27abeafba5588ca74569ba6bebc5d940b767ea3f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824509"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>A Microsoft Intune-ban az Adatszolgáltató regisztrálásával kapcsolatos hibák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
1. Ha az eszköz nem tud regisztrálni, és engedélyezve van az MFA (Multi-Factor Authentication) funkció, tiltsa le az MFA funkciót. Az MFA jelenleg nem támogatott az internetszolgáltató regisztrálása esetén

2. Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.

3. Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják az egyes dokumentumok regisztrálását és [megoldását:](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) [Hibaelhárítási](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) útmutató és Hibaelhárítási dokumentum

4. [További információ az eszközregisztrációs programról.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)
