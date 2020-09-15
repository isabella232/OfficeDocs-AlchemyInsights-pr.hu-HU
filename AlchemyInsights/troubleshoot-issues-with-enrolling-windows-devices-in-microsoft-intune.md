---
title: A Windows-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658880"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="1eebb-102">A Windows-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="1eebb-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="1eebb-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="1eebb-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="1eebb-104">Néhány gyakori hibaüzenet és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="1eebb-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="1eebb-105">**A szoftver nem telepíthető, 0x80cf4017:** Lejárt a fiókja tanúsítványa.</span><span class="sxs-lookup"><span data-stu-id="1eebb-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="1eebb-106">Töltse le újra a PC-kliens szoftvercsomagot az Intune felügyeleti konzolon.</span><span class="sxs-lookup"><span data-stu-id="1eebb-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="1eebb-107">További információért olvassa el ezt a dokumentációt.</span><span class="sxs-lookup"><span data-stu-id="1eebb-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="1eebb-108">**Hibakód 0x801c0003:** A hiba az alábbi esetekben fordulhat elő:</span><span class="sxs-lookup"><span data-stu-id="1eebb-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="1eebb-109">A felhasználó több olyan eszközt regisztrált, mint az eszköz korlátja.</span><span class="sxs-lookup"><span data-stu-id="1eebb-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1eebb-110">Tekintse át ezeket a dokumentumokat az [eszközök eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszköz korlátozásának módosításához](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="1eebb-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="1eebb-111">"A felhasználók az Azure AD-hoz csatlakozhatnak eszközökhöz" beállítás értéke "nincs".</span><span class="sxs-lookup"><span data-stu-id="1eebb-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="1eebb-112">Adja meg az összeset vagy válassza a felhasználók elemet.</span><span class="sxs-lookup"><span data-stu-id="1eebb-112">Set it to all or select users.</span></span> <span data-ttu-id="1eebb-113">További információért olvassa el [ezt a dokumentációt](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="1eebb-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="1eebb-114">Az eszközt már regisztrálta egy másik felhasználó.</span><span class="sxs-lookup"><span data-stu-id="1eebb-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="1eebb-115">Ha ez a helyzet, távolítsa el az eszközt az Azure Intune konzolból, vagy manuálisan távolítsa el az eszközt, és próbálkozzon újra.</span><span class="sxs-lookup"><span data-stu-id="1eebb-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="1eebb-116">Az eszköz a Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="1eebb-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="1eebb-117">Csak a Windows 10 Pro, az oktatási és a vállalati SKU-hoz csatlakozhat az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="1eebb-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="1eebb-118">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="1eebb-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="1eebb-119">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat.</span><span class="sxs-lookup"><span data-stu-id="1eebb-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1eebb-120">További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="1eebb-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="1eebb-121">Tekintse át ezeket a dokumentumokat a tanúsítványigénylést és az állásfoglalásokat akadályozó gyakori hibák listáját: [hibaelhárítási útmutató](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és [Hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="1eebb-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="1eebb-122">[Megtudhatja, hogy miként regisztrálhat Windows-eszközöket a Microsoft Intune-ban](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="1eebb-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
