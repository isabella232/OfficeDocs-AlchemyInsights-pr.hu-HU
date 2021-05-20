---
title: Az eszközkészletből eltávolított vagy leszerelt eszközök eltávolításával kapcsolatos problémák
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564339"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="117f0-102">Az eszközkészletből eltávolított vagy leszerelt eszközök eltávolításával kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="117f0-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="117f0-103">A Microsoft Defender a végponthoz jelenleg nem teszi lehetővé egy kilépett vagy leszerelt eszköz eszközrekordjának manuális eltávolítását az eszközkészletből.</span><span class="sxs-lookup"><span data-stu-id="117f0-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="117f0-104">Biztonsági okokból az eszköz legfeljebb 180 napig marad korábbi rekordként a portálon.</span><span class="sxs-lookup"><span data-stu-id="117f0-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="117f0-105">Az eszköz adatai azonban a beállított megőrzési időnek megfelelően törlődnek.</span><span class="sxs-lookup"><span data-stu-id="117f0-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="117f0-106">**Megjegyzés:** Egy ki van kapcsolva vagy leszerelt eszköz hét nap után automatikusan inaktív állapotba vált. </span><span class="sxs-lookup"><span data-stu-id="117f0-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="117f0-107">Ezenkívül az elmúlt 30 napban nem aktív eszközök nem tükröződik bele az adatokba, amelyek tükrözik a szervezet Veszélyforrás- és biztonságirés-kezelés vagy a Microsoft eszközökre vonatkozó biztonsági pontszámát.</span><span class="sxs-lookup"><span data-stu-id="117f0-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="117f0-108">Ha továbbra sem szeretne bizonyos eszközöket látni az Eszközkészlet nézetben, az Eszközkészlet nézetben próbáljon meg egy eszközcímke elhelyezésével kiszűrni a leszerelt eszközt az Eszközkészlet nézetből.</span><span class="sxs-lookup"><span data-stu-id="117f0-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="117f0-109">További információ:</span><span class="sxs-lookup"><span data-stu-id="117f0-109">For more information, see:</span></span>

[<span data-ttu-id="117f0-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="117f0-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="117f0-111">Expozíciós pontszám a Veszélyforrás- és biztonságirés-kezelés</span><span class="sxs-lookup"><span data-stu-id="117f0-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="117f0-112">Nem belső hibákat figyelő érzékelő kijavítás a Microsoft Defender végponthoz eszközében</span><span class="sxs-lookup"><span data-stu-id="117f0-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="117f0-113">A címkézés hatékony használata (1. rész)</span><span class="sxs-lookup"><span data-stu-id="117f0-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="117f0-114">A címkézés hatékony használata (2. rész)</span><span class="sxs-lookup"><span data-stu-id="117f0-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="117f0-115">A címkézés hatékony használata (3. rész)</span><span class="sxs-lookup"><span data-stu-id="117f0-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




