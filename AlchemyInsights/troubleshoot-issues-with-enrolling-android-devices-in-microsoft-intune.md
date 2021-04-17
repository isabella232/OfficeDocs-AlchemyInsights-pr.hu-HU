---
title: Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830944"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="07e67-102">Az Android-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="07e67-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="07e67-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="07e67-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="07e67-104">Néhány gyakori probléma és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="07e67-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="07e67-105">**Az eszköz nincs titkosítva hibaüzenet a vállalati portálon:** Az Android újabb verziói, különösen a 7.0-s verziótól kezdve, indítókódot igényelnek az eszköz teljes titkosításakor.</span><span class="sxs-lookup"><span data-stu-id="07e67-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="07e67-106">Gyakori megoldás az indítási PIN-kód engedélyezése vagy az eszköz teljes titkosítása.</span><span class="sxs-lookup"><span data-stu-id="07e67-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="07e67-107">További [információért tekintse](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) át ezt a dokumentumot.</span><span class="sxs-lookup"><span data-stu-id="07e67-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="07e67-108">**Az eszközök nem jelennek meg az Intune-szolgáltatásban,** vagy hibásan jelennek meg az Intune felügyeleti konzolján: Egyes Samsung 4.4-es és 5.5-ös eszközök nem biztos, hogy bevetik a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="07e67-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="07e67-109">A problémának három lehetséges megoldása van:</span><span class="sxs-lookup"><span data-stu-id="07e67-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="07e67-110">Nyissa meg manuálisan az Intune Céges portál appot, amely automatikusan elindítja az eszközszinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="07e67-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="07e67-111">Frissítse az eszközt Android 6.0-s vagy újabb verzióra.</span><span class="sxs-lookup"><span data-stu-id="07e67-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="07e67-112">Tiltsa le a Samsung Smart Manager számára az Intune vállalati portál felügyeletét.</span><span class="sxs-lookup"><span data-stu-id="07e67-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="07e67-113">A [dokumentumban további](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) részleteket talál ezekről a problémákról és megoldásukról.</span><span class="sxs-lookup"><span data-stu-id="07e67-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="07e67-114">**Érvénytelen felhasználói licenctípus vagy** Nem felismerhető felhasználónév **hibaüzenet:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni.</span><span class="sxs-lookup"><span data-stu-id="07e67-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="07e67-115">A következő dokumentumok alapján rendeljen licencet: Office Felügyeleti központ vagy Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="07e67-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="07e67-116">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="07e67-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="07e67-117">Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="07e67-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="07e67-118">További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.</span><span class="sxs-lookup"><span data-stu-id="07e67-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="07e67-119">Ebben [a dokumentumban](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) áttekintheti azokat a gyakori hibákat, amelyek meggátolják a regisztrációt és a megoldást az egyes hibákra.</span><span class="sxs-lookup"><span data-stu-id="07e67-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="07e67-120">[Megtudhatja, hogy miként regisztrálható Android-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="07e67-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
