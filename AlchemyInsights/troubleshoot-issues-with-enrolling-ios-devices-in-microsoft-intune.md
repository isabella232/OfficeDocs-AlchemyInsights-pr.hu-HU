---
title: Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294246"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="9446e-102">Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="9446e-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="9446e-103">Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése.</span><span class="sxs-lookup"><span data-stu-id="9446e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="9446e-104">Néhány gyakori hibaüzenetek és a megoldás lépéseit:</span><span class="sxs-lookup"><span data-stu-id="9446e-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="9446e-p101">**Elérhető eszközt kap** A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket. Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/en-us/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.</span><span class="sxs-lookup"><span data-stu-id="9446e-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="9446e-p102">A szolgáltatás **nem támogatott. Nincs tanúsítványigénylési házirend:** Apple leküldéses értesítési szolgáltatás (hozzáférésipont-nevek tartoznak) kell konfigurálni vagy megújítani. [Ez a dokumentum](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) útmutatást ehhez áttekintése.</span><span class="sxs-lookup"><span data-stu-id="9446e-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="9446e-p103">**Felhasználói licenc érvénytelen vagy ismeretlen felhasználónév:** A felhasználónak kell egy Intune vagy EMS licencet kap. Tekintse át ezeket a dokumentumokat keresztül licenc hozzárendelése: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) vagy [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="9446e-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="9446e-111">A probléma megoldásához további erőforrások:</span><span class="sxs-lookup"><span data-stu-id="9446e-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9446e-p104">[Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/en-us/intune/help-desk-operators) további részletekért tekintse át.</span><span class="sxs-lookup"><span data-stu-id="9446e-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="9446e-114">Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9446e-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="9446e-115">[Útmutató a Microsoft Intune iOS-eszközök igénylésére](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="9446e-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

