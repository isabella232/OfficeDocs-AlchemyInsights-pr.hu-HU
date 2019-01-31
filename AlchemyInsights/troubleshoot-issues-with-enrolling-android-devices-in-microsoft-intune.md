---
title: Android-eszköz a Microsoft Intune igénylése problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655885"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="acb3f-102">Android-eszköz a Microsoft Intune igénylése problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="acb3f-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="acb3f-103">Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése.</span><span class="sxs-lookup"><span data-stu-id="acb3f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="acb3f-104">Néhány gyakori problémát, illetve lépéseket:</span><span class="sxs-lookup"><span data-stu-id="acb3f-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="acb3f-p101">**Eszköz nem titkosított hiba a vállalati portál:** Újabb verziói, Android, különösen v7.0, kezdve a rendszerindítási kódot győződjön meg arról, hogy az eszköz teljes mértékben titkosított van szükség. Közös megoldások indító PIN-kód engedélyezése, vagy az eszköz teljes mértékben titkosítja. További információt [a dokumentum](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) áttekintése.</span><span class="sxs-lookup"><span data-stu-id="acb3f-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="acb3f-p102">**Eszközök sikertelen, ellenőrizze a a Intune szolgáltatást, vagy "Unhealthy" a Intune felügyeleti konzolban jeleníti meg:** Néhány Samsung 4.4. és 5.5-ös eszközök nem ellenőrizheti az üzembe helyezés. Van 3 lehetséges megoldás a probléma:</span><span class="sxs-lookup"><span data-stu-id="acb3f-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="acb3f-110">Manuálisan nyissa meg a vállalati portál Intune app, amely automatikusan kezdeményez egy eszköz szinkronizálás.</span><span class="sxs-lookup"><span data-stu-id="acb3f-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="acb3f-111">Az eszköz az Android 6.0-s vagy újabb frissítés.</span><span class="sxs-lookup"><span data-stu-id="acb3f-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="acb3f-p103">Samsung intelligens kezelő letiltása az Intune vállalati portál kezelése. [Ez a dokumentum](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) további részleteket a következő problémák és megoldások áttekintése.</span><span class="sxs-lookup"><span data-stu-id="acb3f-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="acb3f-p104">**Felhasználói licenc típusa érvénytelen** vagy **felhasználói neve ismeretlen hiba:** a felhasználónak kell egy Intune vagy EMS licencet kap. Tekintse át ezeket a dokumentumokat keresztül licenc hozzárendelése: Office Admin Center vagy Azure portal.</span><span class="sxs-lookup"><span data-stu-id="acb3f-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="acb3f-116">A probléma megoldásához további erőforrások:</span><span class="sxs-lookup"><span data-stu-id="acb3f-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="acb3f-p105">[Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/intune/help-desk-operators) további részletekért tekintse át.</span><span class="sxs-lookup"><span data-stu-id="acb3f-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="acb3f-119">Tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listáját.</span><span class="sxs-lookup"><span data-stu-id="acb3f-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="acb3f-120">[Útmutató: Android-eszköz a Microsoft Intune igényelni](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="acb3f-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

