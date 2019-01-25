---
title: Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473585"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="2378e-102">Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="2378e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="2378e-103">Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése.</span><span class="sxs-lookup"><span data-stu-id="2378e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2378e-104">Néhány gyakori hibaüzenetek és a megoldás lépéseit:</span><span class="sxs-lookup"><span data-stu-id="2378e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="2378e-p101">**Nem lehet telepíteni a szoftvert, 0x80cf4017:** A fiók-tanúsítvány lejárt. Töltse le újra a PC-ügyfél szoftvercsomag Intune felügyeleti konzolon. Tekintse át a dokumentációjában talál további információt.</span><span class="sxs-lookup"><span data-stu-id="2378e-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="2378e-108">**0x801c0003 hibakód:** A hiba akkor fordulhat elő, az alábbi esetekben:</span><span class="sxs-lookup"><span data-stu-id="2378e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="2378e-p102">A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket. Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/en-us/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.</span><span class="sxs-lookup"><span data-stu-id="2378e-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="2378e-p103">"Felhasználó csatlakozhat egy eszközök Azure ad" "nincs" értékre van állítva. Állítsa be az összes, vagy válassza ki a felhasználók. [Ez a dokumentáció](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) áttekintése.</span><span class="sxs-lookup"><span data-stu-id="2378e-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="2378e-p104">Az eszköz egy másik felhasználó már részesül. Ez a helyzet, ha az eszköz eltávolítása a Azure Intune konzolról vagy kézzel unenroll az eszköz ismételt próbálkozás előtt.</span><span class="sxs-lookup"><span data-stu-id="2378e-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="2378e-p105">Az eszköz Windows 10 Home. Csak Windows 10 Pro, oktatási és vállalati SKU Azure Active Directory csatlakozhat.</span><span class="sxs-lookup"><span data-stu-id="2378e-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="2378e-118">A probléma megoldásához további erőforrások:</span><span class="sxs-lookup"><span data-stu-id="2378e-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2378e-p106">[Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/en-us/intune/help-desk-operators) további részletekért tekintse át.</span><span class="sxs-lookup"><span data-stu-id="2378e-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2378e-121">Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2378e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="2378e-122">[Útmutató a Windows Microsoft Intune eszközök igénylésére](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="2378e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

