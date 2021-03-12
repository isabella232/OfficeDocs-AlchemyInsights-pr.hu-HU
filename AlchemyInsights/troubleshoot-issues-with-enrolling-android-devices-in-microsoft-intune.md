---
title: Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709000"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d4f64-102">Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="d4f64-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d4f64-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="d4f64-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d4f64-104">Néhány gyakori probléma és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="d4f64-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d4f64-105">**Az eszköz nincs titkosítva hiba a céges portálon:** Az Android újabb verzióinak , különösen a 7.0-s verziótól kezdve, indítási pin-kódra van szükségük ahhoz, hogy az eszköz teljesen titkosított legyen.</span><span class="sxs-lookup"><span data-stu-id="d4f64-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d4f64-106">Gyakori megoldás az indítási pin-kód engedélyezése vagy az eszköz teljes titkosítása.</span><span class="sxs-lookup"><span data-stu-id="d4f64-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d4f64-107">További [információért tekintse](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="d4f64-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d4f64-108">Az eszközök nem jelennek meg az Intune szolgáltatásban, vagy hibásan jelennek meg az **Intune felügyeleti konzolján:** Egyes Samsung 4.4-es és 5.5-ös eszközök nem biztos, hogy bevetik a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="d4f64-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d4f64-109">A problémának három lehetséges megoldása van:</span><span class="sxs-lookup"><span data-stu-id="d4f64-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d4f64-110">Nyissa meg manuálisan az Intune Vállalati portál alkalmazást, amely automatikusan elindítja az eszközszinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="d4f64-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d4f64-111">Frissítse az eszközt Android 6.0-s vagy újabb verzióra.</span><span class="sxs-lookup"><span data-stu-id="d4f64-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d4f64-112">Tiltsa le a Samsung Smart Manager számára az Intune vállalati portál felügyeletét.</span><span class="sxs-lookup"><span data-stu-id="d4f64-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d4f64-113">A [problémaokkal](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) és megoldásokkal kapcsolatos további részletekért tekintse át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="d4f64-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d4f64-114">**Érvénytelen felhasználói licenctípus** vagy nem felismerhető felhasználónév **hiba:** A felhasználónak Intune- vagy EMS-licenccel kell rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="d4f64-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d4f64-115">Tekintse át ezeket a dokumentumokat, és rendeljen licencet a következőn keresztül: Office Felügyeleti központ vagy Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d4f64-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d4f64-116">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="d4f64-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d4f64-117">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="d4f64-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d4f64-118">További [részletekért tekintse](https://docs.microsoft.com/intune/help-desk-operators) át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="d4f64-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d4f64-119">Ebben [a dokumentumban](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) áttekintheti azokat a gyakori hibákat, amelyek meggátolják a regisztrációt és az egyes problémák megoldását.</span><span class="sxs-lookup"><span data-stu-id="d4f64-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d4f64-120">[Megtudhatja, hogy miként regisztrálható Android-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="d4f64-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
