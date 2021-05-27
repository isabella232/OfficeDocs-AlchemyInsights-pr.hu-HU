---
title: Defender végpont ellenőrzése érzékelő állapota
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676178"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="77ccb-102">Defender végpont ellenőrzése érzékelő állapota</span><span class="sxs-lookup"><span data-stu-id="77ccb-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="77ccb-103">Az **Érzékelővel kapcsolatos problémákat** érzékelővel kapcsolatos eszközök csempe a Biztonsági műveletek irányítópulton található.</span><span class="sxs-lookup"><span data-stu-id="77ccb-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="77ccb-104">Ez a csempe információt nyújt arról, hogy az egyes eszközök képesek-e érzékelőadatok biztosítanak és kommunikáljanak a Defender for Endpoint szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="77ccb-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="77ccb-105">Azt jelenti, hogy hány eszköz igényel beavatkozást, és segít azonosítani a problémás eszközöket, és lépéseket tett az ismert problémák kijavítása érdekében.</span><span class="sxs-lookup"><span data-stu-id="77ccb-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="77ccb-106">A csempén két állapotjelző jelzi, hogy hány eszköz nem jelent megfelelően a szolgáltatásnak:</span><span class="sxs-lookup"><span data-stu-id="77ccb-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="77ccb-107">**Misconfigured** Azok az eszközök, amelyek részben jelentik az érzékelő adatait a Defender végpontnak szolgáltatásnak, és javítható konfigurációs hibákat okozhatnak.</span><span class="sxs-lookup"><span data-stu-id="77ccb-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="77ccb-108">**Inaktív** Azok az eszközök, amelyek az elmúlt hónapban több mint hét napja nem jelentek be a Defender végpontszolgáltatásnak.</span><span class="sxs-lookup"><span data-stu-id="77ccb-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="77ccb-109">A csoportok bármelyikére kattintva az Eszközök listához irányítja a rendszer, a választási lehetőségeknek megfelelően szűrve.</span><span class="sxs-lookup"><span data-stu-id="77ccb-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="77ccb-110">Az Eszközök listában az állapotlistát az alábbi állapot szerint szűrheti:</span><span class="sxs-lookup"><span data-stu-id="77ccb-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="77ccb-111">**Aktív** Azok az eszközök, amelyek aktívan bejelentik a Defender a Végpont szolgáltatásnak.</span><span class="sxs-lookup"><span data-stu-id="77ccb-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="77ccb-112">**Misconfigured** Azok az eszközök, amelyek részben jelentéssel látják el az érzékelő adatait a Defender végpontszolgáltatásnak, de kijavítani kell a konfigurációs hibákat.</span><span class="sxs-lookup"><span data-stu-id="77ccb-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="77ccb-113">A helytelenül konfigurált eszközök az alábbi problémák egyikével vagy kombinációjával is problémákat okozhatnak:</span><span class="sxs-lookup"><span data-stu-id="77ccb-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="77ccb-114">Nincsenek érzékelőadatok – Az eszközök leállták az érzékelőadatok küldését.</span><span class="sxs-lookup"><span data-stu-id="77ccb-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="77ccb-115">Korlátozott riasztások indíthatóak el az eszközről.</span><span class="sxs-lookup"><span data-stu-id="77ccb-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="77ccb-116">Károsodott kommunikáció – A készülékkel való kommunikáció károsodott.</span><span class="sxs-lookup"><span data-stu-id="77ccb-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="77ccb-117">Előfordulhat, hogy nem működik a fájlok küldése mély elemzésre, fájlok blokkolása, az eszköz hálózatról való elzárása és az eszközzel való kommunikációt igénylő egyéb műveletek.</span><span class="sxs-lookup"><span data-stu-id="77ccb-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="77ccb-118">**Inaktív** Azok az eszközök, amelyek leálltak a Végpont defender szolgáltatásnak való jelentéssel.</span><span class="sxs-lookup"><span data-stu-id="77ccb-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="77ccb-119">Az Exportálás funkcióval a teljes listát CSV formátumban letöltheti.</span><span class="sxs-lookup"><span data-stu-id="77ccb-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="77ccb-120">További információ: Az érzékelő állapotának [ellenőrzése a Microsoft Defender végponthoz szolgáltatásban.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="77ccb-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="77ccb-121">Ha többet meg nem tudni arról, hogy mi okozta egy eszköz inaktívvá vagy helytelenül van beállítja az eszközt, tekintse meg A nem hibás érzékelőikonok kijavítva a [Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)eszközt.</span><span class="sxs-lookup"><span data-stu-id="77ccb-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
