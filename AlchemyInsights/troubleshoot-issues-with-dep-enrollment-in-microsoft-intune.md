---
title: A DEP-regisztrációval kapcsolatos hibák elhárítása a Microsoft Intune-ban
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797298"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>A DEP-regisztrációval kapcsolatos hibák elhárítása a Microsoft Intune-ban

A probléma megoldásához tekintse át az alábbi forrásokat.
  
1. Ha az adatvégrehajtás-megakadályozási eszköz nem tud regisztrálni és MFA-t (többtényezős hitelesítés), tiltsa le a MFA-t. A DEP-regisztrációk jelenleg nem támogatottak.

2. Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat. További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .

3. Tekintse át ezeket a dokumentumokat a tanúsítványigénylést és az állásfoglalásokat akadályozó gyakori hibák listáját: [hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [Hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. [További információ az eszköz-igénylési programról](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
