---
title: A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708892"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="05df8-102">A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="05df8-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="05df8-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="05df8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="05df8-104">Néhány gyakori hibaüzenet és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="05df8-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="05df8-105">**A szoftver nem telepíthető, és 0x80cf4017:** A fiók tanúsítványa lejárt.</span><span class="sxs-lookup"><span data-stu-id="05df8-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="05df8-106">Töltse le újra a PC-ügyfél szoftvercsomagot az Intune Felügyeleti konzolon.</span><span class="sxs-lookup"><span data-stu-id="05df8-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="05df8-107">További információt ebben a dokumentációban talál.</span><span class="sxs-lookup"><span data-stu-id="05df8-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="05df8-108">**Hibakód 0x801c0003:** A hiba az alábbi esetekben fordulhat elő:</span><span class="sxs-lookup"><span data-stu-id="05df8-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="05df8-109">A felhasználó több eszközt regisztrált, mint az eszközkorlát.</span><span class="sxs-lookup"><span data-stu-id="05df8-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="05df8-110">Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) vagy [módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="05df8-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="05df8-111">A "Felhasználók csatlakozhatnak az Azure AD-hez" beállítás "nincs" beállításra van állítva.</span><span class="sxs-lookup"><span data-stu-id="05df8-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="05df8-112">Állítsa be az összes felhasználót, vagy jelöljön ki felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="05df8-112">Set it to all or select users.</span></span> <span data-ttu-id="05df8-113">További [információt ebben](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) a dokumentációban talál.</span><span class="sxs-lookup"><span data-stu-id="05df8-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="05df8-114">Az eszközt már regisztrálta egy másik felhasználó.</span><span class="sxs-lookup"><span data-stu-id="05df8-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="05df8-115">Ebben az esetben távolítsa el az eszközt az Azure Intune konzolból, vagy manuálisan törölje az eszköz igénylését, mielőtt újra próbálkozik.</span><span class="sxs-lookup"><span data-stu-id="05df8-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="05df8-116">Az eszköz a Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="05df8-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="05df8-117">Az Azure Active Directoryhoz csak Windows 10 Pro, Oktatási és Nagyvállalati verziós SKUs csatlakozhat.</span><span class="sxs-lookup"><span data-stu-id="05df8-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="05df8-118">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="05df8-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="05df8-119">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="05df8-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="05df8-120">További [részletekért tekintse](https://docs.microsoft.com/intune/help-desk-operators) át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="05df8-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="05df8-121">Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, [](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) amelyek meggátolják a regisztrációt és az egyes problémák megoldását: hibaelhárítási útmutató és [hibaelhárítási dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="05df8-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="05df8-122">[Megtudhatja, hogy miként regisztrálja a Windows-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="05df8-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
