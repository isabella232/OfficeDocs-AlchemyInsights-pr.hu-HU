---
title: Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823465"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="70d59-102">Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="70d59-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="70d59-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="70d59-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="70d59-104">Gyakori hibaüzenetek és megoldási lépések:</span><span class="sxs-lookup"><span data-stu-id="70d59-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="70d59-105">**Eszköz cap reached** A felhasználónak több eszköze van regisztrálva, mint az eszközkorlát.</span><span class="sxs-lookup"><span data-stu-id="70d59-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="70d59-106">Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) [vagy módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="70d59-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="70d59-107">**Ez a szolgáltatás nem támogatott. Nincs regisztrációs házirend:** Az Apple leküldéses értesítéseket szolgáltató szolgáltatását konfigurálni vagy meg kell újítani.</span><span class="sxs-lookup"><span data-stu-id="70d59-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="70d59-108">Ennek [utasításokért](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) tekintse át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="70d59-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="70d59-109">**Érvénytelen felhasználói licenctípus, vagy nem ismerhető fel a felhasználónév:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni.</span><span class="sxs-lookup"><span data-stu-id="70d59-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="70d59-110">A következő dokumentumok alapján rendeljen licencet: [Office Felügyeleti központ](https://docs.microsoft.com/intune/licenses-assign) vagy Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="70d59-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="70d59-111">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="70d59-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="70d59-112">Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="70d59-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="70d59-113">További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.</span><span class="sxs-lookup"><span data-stu-id="70d59-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="70d59-114">Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják az egyes dokumentumok regisztrálását és megoldását: [Hibaelhárítási](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) útmutató és Hibaelhárítási [dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="70d59-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="70d59-115">[Megtudhatja, hogy miként regisztrálható az iOS-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="70d59-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

