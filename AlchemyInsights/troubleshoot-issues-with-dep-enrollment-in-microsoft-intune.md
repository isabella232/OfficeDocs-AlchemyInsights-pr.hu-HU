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
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="b92af-102">A Microsoft Intune-ban való dep-regisztrációval kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="b92af-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="b92af-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="b92af-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="b92af-104">Ha az adatsorkezelő eszköz nem tud beiratkozni, és az MFA (Multi-Factor Authentication) engedélyezve van, tiltsa le az MFA-t.</span><span class="sxs-lookup"><span data-stu-id="b92af-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="b92af-105">Jelenleg az MFA nem támogatott az dep-regisztrációhoz</span><span class="sxs-lookup"><span data-stu-id="b92af-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="b92af-106">Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="b92af-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b92af-107">Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért.</span><span class="sxs-lookup"><span data-stu-id="b92af-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="b92af-108">Tekintse át ezeket a dokumentumokat a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és az egyes megoldásokat: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [hibaelhárítás idopont](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="b92af-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="b92af-109">[További információ az eszközregisztrációs programról.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="b92af-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
