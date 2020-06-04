---
title: A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665834"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="8b65d-102">A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="8b65d-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="8b65d-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="8b65d-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="8b65d-104">Néhány gyakori hibaüzenet és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="8b65d-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="8b65d-105">**A szoftver nem telepíthető, 0x80cf4017:** A fióktanúsítvány lejárt.</span><span class="sxs-lookup"><span data-stu-id="8b65d-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="8b65d-106">Töltse le újra a PC-ügyfél szoftvercsomagot az Intune felügyeleti konzolján.</span><span class="sxs-lookup"><span data-stu-id="8b65d-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="8b65d-107">További információkért tekintse át ezt a dokumentációt.</span><span class="sxs-lookup"><span data-stu-id="8b65d-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="8b65d-108">**0x801c0003 hibakód:** A hiba a következő esetekben fordulhat elő:</span><span class="sxs-lookup"><span data-stu-id="8b65d-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="8b65d-109">A felhasználó több eszközt regisztrált, mint az eszköz korlátját.</span><span class="sxs-lookup"><span data-stu-id="8b65d-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8b65d-110">Tekintse át ezeket a dokumentumokat [az eszköz eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszközkorlát módosításához.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="8b65d-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="8b65d-111">"A felhasználók csatlakozhatnak az Azure AD-hez" beállítás "nincs" lesz.</span><span class="sxs-lookup"><span data-stu-id="8b65d-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="8b65d-112">Állítsa be az összes, vagy válassza ki a felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="8b65d-112">Set it to all or select users.</span></span> <span data-ttu-id="8b65d-113">További információkért tekintse át ezt a [dokumentációt.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)</span><span class="sxs-lookup"><span data-stu-id="8b65d-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="8b65d-114">Az eszközt már regisztrálta egy másik felhasználó.</span><span class="sxs-lookup"><span data-stu-id="8b65d-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="8b65d-115">Ebben az esetben távolítsa el az eszközt az Azure Intune konzolról, vagy manuálisan szüntesse meg az eszközt, mielőtt újra próbálkozna.</span><span class="sxs-lookup"><span data-stu-id="8b65d-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="8b65d-116">Az eszköz a Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="8b65d-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="8b65d-117">Csak a Windows 10 Pro, oktatási és nagyvállalati ska-k csatlakozhatnak az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="8b65d-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="8b65d-118">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="8b65d-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="8b65d-119">Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="8b65d-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8b65d-120">Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért.</span><span class="sxs-lookup"><span data-stu-id="8b65d-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="8b65d-121">Tekintse át ezeket a dokumentumokat a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és az egyes megoldásokat: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és [hibaelhárítás idopont](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8b65d-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="8b65d-122">[Megtudhatja, hogy miként regisztrálhat Windows-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="8b65d-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
