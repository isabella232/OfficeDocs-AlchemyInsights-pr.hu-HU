---
title: IOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736160"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="3df4c-102">IOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="3df4c-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="3df4c-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="3df4c-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="3df4c-104">Néhány gyakori hibaüzenet és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="3df4c-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="3df4c-105">**Elérte az eszközkorlátot** A felhasználó több eszközt regisztrált, mint az eszköz korlátját.</span><span class="sxs-lookup"><span data-stu-id="3df4c-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3df4c-106">Tekintse át ezeket a dokumentumokat [az eszköz eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszközkorlát módosításához.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="3df4c-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="3df4c-107">**Ez a szolgáltatás nem támogatott. Nincs regisztrációs szabályzat:** Az Apple leküldéses értesítési szolgáltatását (APNS) konfigurálni vagy megújítani kell.</span><span class="sxs-lookup"><span data-stu-id="3df4c-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="3df4c-108">Tekintse át ezt a [dokumentumot,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) hogy ennek hogyan tehető.</span><span class="sxs-lookup"><span data-stu-id="3df4c-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="3df4c-109">**Érvénytelen felhasználói licenctípus vagy nem felismert felhasználónév:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelnie.</span><span class="sxs-lookup"><span data-stu-id="3df4c-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3df4c-110">Tekintse át ezeket a dokumentumokat, hogy licencet rendeljen az [Office Felügyeleti központon](https://docs.microsoft.com/intune/licenses-assign) vagy [az Azure Portalon](https://docs.microsoft.com/azure/active-directory/license-users-groups)keresztül.</span><span class="sxs-lookup"><span data-stu-id="3df4c-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="3df4c-111">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="3df4c-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3df4c-112">Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="3df4c-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3df4c-113">Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért.</span><span class="sxs-lookup"><span data-stu-id="3df4c-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="3df4c-114">Tekintse át ezeket a dokumentumokat a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és az egyes megoldásokat: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [hibaelhárítás idopont](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="3df4c-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="3df4c-115">[Megtudhatja, hogy miként regisztrálhatja az iOS-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="3df4c-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

