---
title: Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559663"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="75a10-102">Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="75a10-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="75a10-103">Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése.</span><span class="sxs-lookup"><span data-stu-id="75a10-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="75a10-104">Néhány gyakori hibaüzenetek és a megoldás lépéseit:</span><span class="sxs-lookup"><span data-stu-id="75a10-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="75a10-105">**Nem lehet telepíteni a szoftvert, 0x80cf4017:** A fiók-tanúsítvány lejárt.</span><span class="sxs-lookup"><span data-stu-id="75a10-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="75a10-106">Töltse le újra a PC-ügyfél szoftvercsomag Intune felügyeleti konzolon.</span><span class="sxs-lookup"><span data-stu-id="75a10-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="75a10-107">Tekintse át a dokumentációjában talál további információt.</span><span class="sxs-lookup"><span data-stu-id="75a10-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="75a10-108">**0x801c0003 hibakód:** A hiba akkor fordulhat elő, az alábbi esetekben:</span><span class="sxs-lookup"><span data-stu-id="75a10-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="75a10-109">A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket.</span><span class="sxs-lookup"><span data-stu-id="75a10-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="75a10-110">Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.</span><span class="sxs-lookup"><span data-stu-id="75a10-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="75a10-111">"Felhasználó csatlakozhat egy eszközök Azure ad" "nincs" értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="75a10-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="75a10-112">Állítsa be az összes, vagy válassza ki a felhasználók.</span><span class="sxs-lookup"><span data-stu-id="75a10-112">Set it to all or select users.</span></span> <span data-ttu-id="75a10-113">[Ez a dokumentáció](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) áttekintése.</span><span class="sxs-lookup"><span data-stu-id="75a10-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="75a10-114">Az eszköz egy másik felhasználó már részesül.</span><span class="sxs-lookup"><span data-stu-id="75a10-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="75a10-115">Ez a helyzet, ha az eszköz eltávolítása a Azure Intune konzolról vagy kézzel unenroll az eszköz ismételt próbálkozás előtt.</span><span class="sxs-lookup"><span data-stu-id="75a10-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="75a10-116">Az eszköz Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="75a10-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="75a10-117">Csak Windows 10 Pro, oktatási és vállalati SKU Azure Active Directory csatlakozhat.</span><span class="sxs-lookup"><span data-stu-id="75a10-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="75a10-118">A probléma megoldásához további erőforrások:</span><span class="sxs-lookup"><span data-stu-id="75a10-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="75a10-119">[Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák.</span><span class="sxs-lookup"><span data-stu-id="75a10-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="75a10-120">[Ez a dokumentum](https://docs.microsoft.com/intune/help-desk-operators) további részletekért tekintse át.</span><span class="sxs-lookup"><span data-stu-id="75a10-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="75a10-121">Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="75a10-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="75a10-122">[Útmutató a Windows Microsoft Intune eszközök igénylésére](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="75a10-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
