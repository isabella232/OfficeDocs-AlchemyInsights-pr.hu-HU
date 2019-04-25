---
title: Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391009"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="ad652-102">Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="ad652-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="ad652-103">Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése.</span><span class="sxs-lookup"><span data-stu-id="ad652-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="ad652-104">Néhány gyakori hibaüzenetek és a megoldás lépéseit:</span><span class="sxs-lookup"><span data-stu-id="ad652-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="ad652-105">**Elérhető eszközt kap** A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket.</span><span class="sxs-lookup"><span data-stu-id="ad652-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="ad652-106">Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.</span><span class="sxs-lookup"><span data-stu-id="ad652-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="ad652-107">A szolgáltatás **nem támogatott. Nincs tanúsítványigénylési házirend:** Apple leküldéses értesítési szolgáltatás (hozzáférésipont-nevek tartoznak) kell konfigurálni vagy megújítani.</span><span class="sxs-lookup"><span data-stu-id="ad652-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="ad652-108">[Ez a dokumentum](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) útmutatást ehhez áttekintése.</span><span class="sxs-lookup"><span data-stu-id="ad652-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="ad652-109">**Felhasználói licenc érvénytelen vagy ismeretlen felhasználónév:** A felhasználónak kell egy Intune vagy EMS licencet kap.</span><span class="sxs-lookup"><span data-stu-id="ad652-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ad652-110">Tekintse át ezeket a dokumentumokat keresztül licenc hozzárendelése: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) vagy [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="ad652-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="ad652-111">A probléma megoldásához további erőforrások:</span><span class="sxs-lookup"><span data-stu-id="ad652-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ad652-112">[Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák.</span><span class="sxs-lookup"><span data-stu-id="ad652-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ad652-113">[Ez a dokumentum](https://docs.microsoft.com/intune/help-desk-operators) további részletekért tekintse át.</span><span class="sxs-lookup"><span data-stu-id="ad652-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ad652-114">Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ad652-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="ad652-115">[Útmutató a Microsoft Intune iOS-eszközök igénylésére](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="ad652-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

