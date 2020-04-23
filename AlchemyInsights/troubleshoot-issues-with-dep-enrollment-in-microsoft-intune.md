---
title: A Microsoft Intune-ban való dep-regisztrációval kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 11b0d73c34996fd84431b38d77b64536d386977e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766711"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>A Microsoft Intune-ban való dep-regisztrációval kapcsolatos problémák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
1. Ha az adatsorkezelő eszköz nem tud beiratkozni, és az MFA (Multi-Factor Authentication) engedélyezve van, tiltsa le az MFA-t. Jelenleg az MFA nem támogatott az dep-regisztrációhoz

2. Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat. Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért.

3. Tekintse át ezeket a dokumentumokat a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és az egyes megoldásokat: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [hibaelhárítás idopont](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. [További információ az eszközregisztrációs programról.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)
