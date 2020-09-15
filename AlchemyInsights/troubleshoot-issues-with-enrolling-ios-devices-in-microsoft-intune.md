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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>IOS-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat. 
  
Néhány gyakori hibaüzenet és megoldási lépés:
  
- **Eszköz sapka elérte** A felhasználó több olyan eszközt regisztrált, mint az eszköz korlátja. Tekintse át ezeket a dokumentumokat az [eszközök eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszköz korlátozásának módosításához](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ez a szolgáltatás nem támogatott. Nincs tanúsítványigénylési házirend:** az Apple leküldéses értesítési szolgáltatást (APNS) be kell állítani vagy meg kell újítani. Nézze át [ezt a dokumentumot](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , ha szeretne útmutatást csinálni. 
    
- A **felhasználói licenc típusa érvénytelen, vagy a Felhasználónév nem ismerhető fel:** A felhasználónak Intune vagy EMS licencet kell rendelnie. Ezekkel a dokumentumokkal az [Office felügyeleti központból](https://docs.microsoft.com/intune/licenses-assign) vagy az [Azure portálról](https://docs.microsoft.com/azure/active-directory/license-users-groups)rendelhet licencet:
    
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat. További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Tekintse át ezeket a dokumentumokat a tanúsítványigénylést és az állásfoglalásokat akadályozó gyakori hibák listáját: [hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [Hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Megtudhatja, hogy miként regisztrálhat iOS-eszközöket a Microsoft Intune-ban](https://docs.microsoft.com/intune/ios-enroll).
    

