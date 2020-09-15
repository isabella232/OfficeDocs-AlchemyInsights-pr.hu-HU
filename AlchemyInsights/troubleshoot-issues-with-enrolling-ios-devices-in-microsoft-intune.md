---
title: IOS-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása
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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669250"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="97e6b-102">IOS-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="97e6b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="97e6b-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="97e6b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="97e6b-104">Néhány gyakori hibaüzenet és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="97e6b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="97e6b-105">**Eszköz sapka elérte** A felhasználó több olyan eszközt regisztrált, mint az eszköz korlátja.</span><span class="sxs-lookup"><span data-stu-id="97e6b-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="97e6b-106">Tekintse át ezeket a dokumentumokat az [eszközök eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszköz korlátozásának módosításához](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="97e6b-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="97e6b-107">**Ez a szolgáltatás nem támogatott. Nincs tanúsítványigénylési házirend:** az Apple leküldéses értesítési szolgáltatást (APNS) be kell állítani vagy meg kell újítani.</span><span class="sxs-lookup"><span data-stu-id="97e6b-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="97e6b-108">Nézze át [ezt a dokumentumot](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , ha szeretne útmutatást csinálni.</span><span class="sxs-lookup"><span data-stu-id="97e6b-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="97e6b-109">A **felhasználói licenc típusa érvénytelen, vagy a Felhasználónév nem ismerhető fel:** A felhasználónak Intune vagy EMS licencet kell rendelnie.</span><span class="sxs-lookup"><span data-stu-id="97e6b-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="97e6b-110">Ezekkel a dokumentumokkal az [Office felügyeleti központból](https://docs.microsoft.com/intune/licenses-assign) vagy az [Azure portálról](https://docs.microsoft.com/azure/active-directory/license-users-groups)rendelhet licencet:</span><span class="sxs-lookup"><span data-stu-id="97e6b-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="97e6b-111">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="97e6b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="97e6b-112">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat.</span><span class="sxs-lookup"><span data-stu-id="97e6b-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="97e6b-113">További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="97e6b-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="97e6b-114">Tekintse át ezeket a dokumentumokat a tanúsítványigénylést és az állásfoglalásokat akadályozó gyakori hibák listáját: [hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [Hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="97e6b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="97e6b-115">[Megtudhatja, hogy miként regisztrálhat iOS-eszközöket a Microsoft Intune-ban](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="97e6b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

