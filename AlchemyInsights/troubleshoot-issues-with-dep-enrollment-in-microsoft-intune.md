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
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="99d8b-102">A DEP-regisztrációval kapcsolatos hibák elhárítása a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="99d8b-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="99d8b-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="99d8b-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="99d8b-104">Ha az adatvégrehajtás-megakadályozási eszköz nem tud regisztrálni és MFA-t (többtényezős hitelesítés), tiltsa le a MFA-t.</span><span class="sxs-lookup"><span data-stu-id="99d8b-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="99d8b-105">A DEP-regisztrációk jelenleg nem támogatottak.</span><span class="sxs-lookup"><span data-stu-id="99d8b-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="99d8b-106">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat.</span><span class="sxs-lookup"><span data-stu-id="99d8b-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="99d8b-107">További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="99d8b-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="99d8b-108">Tekintse át ezeket a dokumentumokat a tanúsítványigénylést és az állásfoglalásokat akadályozó gyakori hibák listáját: [hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [Hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="99d8b-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="99d8b-109">[További információ az eszköz-igénylési programról](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="99d8b-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
