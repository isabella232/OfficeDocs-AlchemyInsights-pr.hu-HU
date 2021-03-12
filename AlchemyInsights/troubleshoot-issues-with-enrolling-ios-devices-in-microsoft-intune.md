---
title: Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708964"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="1c10d-102">Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="1c10d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="1c10d-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="1c10d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="1c10d-104">Néhány gyakori hibaüzenet és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="1c10d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="1c10d-105">**Eszköz cap reached** A felhasználó több eszközt regisztrált, mint az eszközkorlát.</span><span class="sxs-lookup"><span data-stu-id="1c10d-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1c10d-106">Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) vagy [módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="1c10d-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="1c10d-107">**Ez a szolgáltatás nem támogatott. Nincs regisztrációs házirend:** Az Apple leküldéses értesítési szolgáltatását (APNS) konfigurálni vagy meg kell újítani.</span><span class="sxs-lookup"><span data-stu-id="1c10d-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="1c10d-108">Ennek [mikéntjére](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) vonatkozó utasításokat ebben a dokumentumban tud meg.</span><span class="sxs-lookup"><span data-stu-id="1c10d-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="1c10d-109">**A felhasználói licenc típusa érvénytelen vagy a felhasználónév nem ismerhető fel:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni.</span><span class="sxs-lookup"><span data-stu-id="1c10d-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="1c10d-110">Tekintse át az alábbi dokumentumokat, és rendeljen licencet a következőn keresztül: [Office Felügyeleti központ](https://docs.microsoft.com/intune/licenses-assign) vagy Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="1c10d-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="1c10d-111">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="1c10d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1c10d-112">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="1c10d-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1c10d-113">További [részletekért tekintse](https://docs.microsoft.com/intune/help-desk-operators) át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="1c10d-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1c10d-114">Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, [](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) amelyek meggátolják a regisztrációt és az egyes problémák megoldását: hibaelhárítási útmutató és [hibaelhárítási dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="1c10d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="1c10d-115">[Megtudhatja, hogy miként regisztrálható iOS-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="1c10d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

