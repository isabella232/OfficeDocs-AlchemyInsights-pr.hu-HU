---
title: A Microsoft Intune-ban való adatszolgáltató-regisztrációval kapcsolatos hibák elhárítása
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
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708712"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="b5a13-102">A Microsoft Intune-ban való adatszolgáltató-regisztrációval kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="b5a13-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="b5a13-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="b5a13-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="b5a13-104">Ha az eszköz nem tud regisztrálni, és az MFA (Multi-Factor Authentication) engedélyezve van, tiltsa le az MFA funkciót.</span><span class="sxs-lookup"><span data-stu-id="b5a13-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="b5a13-105">Az MFA jelenleg nem támogatott az internetszolgáltató regisztrációja esetén</span><span class="sxs-lookup"><span data-stu-id="b5a13-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="b5a13-106">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="b5a13-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b5a13-107">További [részletekért tekintse](https://docs.microsoft.com/intune/help-desk-operators) át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="b5a13-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="b5a13-108">Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják a regisztrációt és a felbontást [az](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) egyes [dokumentumokban:](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Hibaelhárítási útmutató és hibaelhárítási dokumentum</span><span class="sxs-lookup"><span data-stu-id="b5a13-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="b5a13-109">[További információ az eszközregisztrációs programról.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="b5a13-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
