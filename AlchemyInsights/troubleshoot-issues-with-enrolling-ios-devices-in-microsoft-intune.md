---
title: IOS-eszközökkel kapcsolatos problémák elhárítása a Microsoft Intune-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507005"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e0306-102">IOS-eszközökkel kapcsolatos problémák elhárítása a Microsoft Intune-ben</span><span class="sxs-lookup"><span data-stu-id="e0306-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e0306-103">A probléma megoldásához tekintse át az alább felsorolt erőforrásokat.</span><span class="sxs-lookup"><span data-stu-id="e0306-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e0306-104">Gyakori hibaüzenetek és megoldási lépések:</span><span class="sxs-lookup"><span data-stu-id="e0306-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e0306-105">A **Device Cap elérte** A felhasználó több, az eszközkorlátnál igényléssel rendelkező eszközzel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="e0306-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e0306-106">Ellenőrizze ezeket a dokumentumokat az [eszköz eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszközkorlát megváltoztatásához](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="e0306-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e0306-107">**Ez a szolgáltatás nem támogatott. Nem besorozás politika:** Alma támadás hirdetés szolgáltatás (APNS) szükséges-hoz lenni configured vagy megújít.</span><span class="sxs-lookup"><span data-stu-id="e0306-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e0306-108">Olvassa el [ezt a dokumentumot](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , hogy hogyan kell ezt megtenni.</span><span class="sxs-lookup"><span data-stu-id="e0306-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e0306-109">**Érvénytelen felhasználói licenctípus, vagy a felhasználó neve nem ismerhető fel:** A felhasználónak Intune-vagy EMS-licencet kell rendelni.</span><span class="sxs-lookup"><span data-stu-id="e0306-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e0306-110">Tekintse át ezeket a dokumentumokat, és rendeljen hozzá licencet az [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) vagy az [Azure Portal webhelyen](https://docs.microsoft.com/azure/active-directory/license-users-groups)keresztül.</span><span class="sxs-lookup"><span data-stu-id="e0306-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e0306-111">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="e0306-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e0306-112">Az [Intune – hibaelhárítás portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) használatával diagnosztizálhatja és megoldhatja a gyakori igénylési hibákat.</span><span class="sxs-lookup"><span data-stu-id="e0306-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e0306-113">További részletekért olvassa el [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="e0306-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e0306-114">Tekintse át ezeket a dokumentumokat az olyan gyakori hibák listájához, amelyek megakadályozzák a tanúsítványigénylést és az egyes felbontásokat: [hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és a [doc-hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e0306-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e0306-115">[Információ az iOS-eszközök Microsoft Intune szolgáltatással történő igényléséről](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="e0306-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

