---
title: Az Office 365-be való deszkálással kapcsolatos Microsoft Intune
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
ms.openlocfilehash: e77295f0395919a723dcec1a313ca03154ae59b1bea22bf791f3a0f923cab60d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008260"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Az Office 365-be való deszkálással kapcsolatos Microsoft Intune

A probléma megoldásához tekintse át az alábbi forrásokat.
  
1. Ha az eszköz nem tud regisztrálni, és engedélyezve van az MFA (Multi-Factor Authentication) funkció, tiltsa le az MFA funkciót. Az MFA jelenleg nem támogatott az internetszolgáltató regisztrálása esetén

2. Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.

3. Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják az egyes dokumentumok regisztrálását és [megoldását:](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) [Hibaelhárítási](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) útmutató és Hibaelhárítási dokumentum

4. [További információ az eszközregisztrációs programról.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)
