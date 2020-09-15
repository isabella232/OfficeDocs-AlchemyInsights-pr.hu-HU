---
title: Az Android-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689956"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="17749-102">Az Android-eszközök Microsoft Intune-ban való igénylésével kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="17749-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="17749-103">A probléma megoldásához tekintse át az alábbi forrásokat.</span><span class="sxs-lookup"><span data-stu-id="17749-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="17749-104">Néhány gyakori probléma és megoldási lépés:</span><span class="sxs-lookup"><span data-stu-id="17749-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="17749-105">**A vállalati portál eszköz nem titkosított hibája:** Az Android újabb verzióihoz, különösen a v 7.0-s verziójához, indítási hitelesítő kód szükséges ahhoz, hogy az eszköz teljes mértékben titkosítva legyen.</span><span class="sxs-lookup"><span data-stu-id="17749-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="17749-106">A gyakori megoldásokkal engedélyezheti az indítási PIN-kódot, vagy teljes mértékben titkosíthatja az eszközt.</span><span class="sxs-lookup"><span data-stu-id="17749-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="17749-107">További információt a [dokumentum](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) véleményezése című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="17749-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="17749-108">**Az Intune felügyeleti konzoljában az eszközök nem jelennek meg a Intune szolgáltatással, vagy a "nem egészséges" megjelenítéssel:** Előfordulhat, hogy egyes Samsung 4,4-és 5,5-eszközök nem kerülnek be a szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="17749-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="17749-109">Ebből a problémából 3 lehetséges megoldás áll rendelkezésre:</span><span class="sxs-lookup"><span data-stu-id="17749-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="17749-110">Nyissa meg manuálisan az Intune vállalati portál alkalmazást, amely automatikusan elindítja az eszköz szinkronizálását.</span><span class="sxs-lookup"><span data-stu-id="17749-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="17749-111">Frissítse az eszközt Android 6,0-es vagy újabb verzióra.</span><span class="sxs-lookup"><span data-stu-id="17749-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="17749-112">Tiltsa le a Samsung Smart Managert az Intune vállalati portál kezelésének letiltásával.</span><span class="sxs-lookup"><span data-stu-id="17749-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="17749-113">Tekintse át a következő témakört, és olvassa el a fenti problémákat és állásfoglalásokat ismertető [dokumentumot](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) .</span><span class="sxs-lookup"><span data-stu-id="17749-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="17749-114">A **felhasználói licenc típusa érvénytelen** vagy a **Felhasználónév nem ismerhető fel hiba:** a felhasználónak Intune vagy EMS licenccel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="17749-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="17749-115">Ezekkel a dokumentumokkal az Office felügyeleti központból vagy az Azure portálról rendelhet licencet:</span><span class="sxs-lookup"><span data-stu-id="17749-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="17749-116">További források a probléma megoldásához:</span><span class="sxs-lookup"><span data-stu-id="17749-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="17749-117">Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) megkeresheti és megoldhatja a gyakori beiktatási hibákat.</span><span class="sxs-lookup"><span data-stu-id="17749-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="17749-118">További részletekért tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="17749-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="17749-119">Tekintse át [ezt a dokumentumot](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) azoknak a gyakori hibáknak a listáját, amelyekkel megelőzheti a beiratkozási és a felbontást.</span><span class="sxs-lookup"><span data-stu-id="17749-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="17749-120">[Megtudhatja, hogy miként regisztrálhat Android-eszközöket a Microsoft Intune-ban](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="17749-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
