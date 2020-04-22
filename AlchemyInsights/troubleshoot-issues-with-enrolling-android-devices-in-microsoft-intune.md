---
title: Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759622"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="87627-102">Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="87627-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="87627-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="87627-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="87627-104">Néhány gyakori probléma és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="87627-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="87627-105">**Az eszköz nem titkosított hiba a céges portálon:** Az Android újabb verziói, különösen a 7.0-s verzióval kezdve, indítási jelkódot igényelnek annak érdekében, hogy az eszköz teljesen titkosítva legyen.</span><span class="sxs-lookup"><span data-stu-id="87627-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="87627-106">A gyakori megoldások az indítópin engedélyezése vagy az eszköz teljes titkosítása.</span><span class="sxs-lookup"><span data-stu-id="87627-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="87627-107">További információkért tekintse át ezt a [dokumentumot.](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)</span><span class="sxs-lookup"><span data-stu-id="87627-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="87627-108">**Az eszközök nem jelentkeznek be az Intune szolgáltatással, vagy "Nem kifogástalan" állapotúként jelennek meg az Intune felügyeleti konzolján:** Előfordulhat, hogy egyes Samsung 4.4 és 5.5 eszközök nem jelentkeznek be a szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="87627-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="87627-109">A probléma 3 lehetséges megoldása lehetséges:</span><span class="sxs-lookup"><span data-stu-id="87627-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="87627-110">Manuálisan nyissa meg az Intune Céges portál alkalmazást, amely automatikusan elindítja az eszközszinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="87627-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="87627-111">Frissítse az eszközt Android 6.0-s vagy újabb verzióra.</span><span class="sxs-lookup"><span data-stu-id="87627-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="87627-112">Tiltsa le a Samsung Smart Manager t az Intune vállalati portáljának kezelésében.</span><span class="sxs-lookup"><span data-stu-id="87627-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="87627-113">Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) a további részletekért ezekről a kérdésekről és állásfoglalásokról.</span><span class="sxs-lookup"><span data-stu-id="87627-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="87627-114">**Érvénytelen felhasználói licenctípus** vagy **nem felismert felhasználónév hiba:** A felhasználóhoz Intune- vagy EMS-licencet kell rendelni.</span><span class="sxs-lookup"><span data-stu-id="87627-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="87627-115">Tekintse át ezeket a dokumentumokat, hogy licencet rendeljen az Office Felügyeleti központon vagy az Azure Portalon keresztül.</span><span class="sxs-lookup"><span data-stu-id="87627-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="87627-116">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="87627-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="87627-117">Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="87627-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="87627-118">Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért.</span><span class="sxs-lookup"><span data-stu-id="87627-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="87627-119">Tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és a megoldásokat.</span><span class="sxs-lookup"><span data-stu-id="87627-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="87627-120">[Megtudhatja, hogy miként regisztrálhat Android-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="87627-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
