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
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="60223-102">A Microsoft Intune-ban az Adatszolgáltató regisztrálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="60223-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="60223-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="60223-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="60223-104">Ha az eszköz nem tud regisztrálni, és engedélyezve van az MFA (Multi-Factor Authentication) funkció, tiltsa le az MFA funkciót.</span><span class="sxs-lookup"><span data-stu-id="60223-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="60223-105">Az MFA jelenleg nem támogatott az internetszolgáltató regisztrálása esetén</span><span class="sxs-lookup"><span data-stu-id="60223-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="60223-106">Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="60223-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="60223-107">További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.</span><span class="sxs-lookup"><span data-stu-id="60223-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="60223-108">Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják az egyes dokumentumok regisztrálását és [megoldását:](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) [Hibaelhárítási](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) útmutató és Hibaelhárítási dokumentum</span><span class="sxs-lookup"><span data-stu-id="60223-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="60223-109">[További információ az eszközregisztrációs programról.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="60223-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
