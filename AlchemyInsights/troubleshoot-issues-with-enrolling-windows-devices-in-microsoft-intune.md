---
title: A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808973"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="41f07-102">A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="41f07-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="41f07-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="41f07-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="41f07-104">Gyakori hibaüzenetek és megoldási lépések:</span><span class="sxs-lookup"><span data-stu-id="41f07-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="41f07-105">**A szoftvert nem lehet telepíteni, mert ez 0x80cf4017:** A fiók tanúsítványa lejárt.</span><span class="sxs-lookup"><span data-stu-id="41f07-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="41f07-106">Töltse le újra a PC-ügyfélszoftver csomagját az Intune Felügyeleti konzolon.</span><span class="sxs-lookup"><span data-stu-id="41f07-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="41f07-107">További információt ebben a dokumentációban talál.</span><span class="sxs-lookup"><span data-stu-id="41f07-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="41f07-108">**Hibakód 0x801c0003:** A hiba az alábbi esetekben fordulhat elő:</span><span class="sxs-lookup"><span data-stu-id="41f07-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="41f07-109">A felhasználónak több eszköze van regisztrálva, mint az eszközkorlát.</span><span class="sxs-lookup"><span data-stu-id="41f07-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="41f07-110">Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) [vagy módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="41f07-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="41f07-111">A "Felhasználók csatlakozhatnak az Azure AD-hez" beállítás "nincs" beállításra van állítva.</span><span class="sxs-lookup"><span data-stu-id="41f07-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="41f07-112">Állítsa be az összes felhasználóra, vagy válassza ki a kívánt felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="41f07-112">Set it to all or select users.</span></span> <span data-ttu-id="41f07-113">További [információt ebben](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) a dokumentációban talál.</span><span class="sxs-lookup"><span data-stu-id="41f07-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="41f07-114">Az eszközt már regisztrálta egy másik felhasználó.</span><span class="sxs-lookup"><span data-stu-id="41f07-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="41f07-115">Ha ez a helyzet, távolítsa el az eszközt az Azure Intune konzolból, vagy manuálisan törölje az eszköz igénylését, mielőtt újra próbálkozik.</span><span class="sxs-lookup"><span data-stu-id="41f07-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="41f07-116">Az eszköz a Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="41f07-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="41f07-117">Csak a Windows 10 Pro, az Oktatási és a Nagyvállalati verziós előfizetések csatlakozhatnak az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="41f07-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="41f07-118">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="41f07-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="41f07-119">Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="41f07-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="41f07-120">További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.</span><span class="sxs-lookup"><span data-stu-id="41f07-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="41f07-121">Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják az egyes dokumentumok regisztrálását és megoldását: [Hibaelhárítási](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) útmutató és Hibaelhárítási [dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="41f07-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="41f07-122">[Megtudhatja, hogy miként regisztrálja a Windows-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="41f07-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
