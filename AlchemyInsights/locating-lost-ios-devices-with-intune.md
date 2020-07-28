---
title: Elveszett iOS-eszközök megkeresése az Intune-nal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439627"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="97025-102">Elveszett iOS-eszközök megkeresése az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="97025-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="97025-103">Az elveszett mód engedélyezése iOS-eszközön lehetővé teszi a rendszergazda számára, hogy egy üzenet és a kapcsolattartó telefonszáma megjelenjen a zárolási képernyőn.</span><span class="sxs-lookup"><span data-stu-id="97025-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="97025-104">Az elveszett mód engedélyezése után a rendszergazda az Eszköz megkeresése művelettel azonosíthatja az eszköz fizikai helyét.</span><span class="sxs-lookup"><span data-stu-id="97025-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="97025-105">Az Eszköz megkeresése művelet az Intune-ban együttműködik az iOS-eszközökkel egy adott eszköz helyének megjelenítéséhez a térképen.</span><span class="sxs-lookup"><span data-stu-id="97025-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="97025-106">A művelet használatához az iOS-készüléknek a következőkben kell lennie:</span><span class="sxs-lookup"><span data-stu-id="97025-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="97025-107">Felügyelt mód</span><span class="sxs-lookup"><span data-stu-id="97025-107">Supervised mode</span></span>
- <span data-ttu-id="97025-108">Elveszett mód</span><span class="sxs-lookup"><span data-stu-id="97025-108">Lost mode</span></span>

<span data-ttu-id="97025-109">További információ: [Elveszett mód engedélyezése iOS/iPadOS eszközökön az Intune-nal,](https://docs.microsoft.com/intune/device-lost-mode) és [az elveszett vagy ellopott iOS/iPadOS-eszközök megkeresése az Intune-nal.](https://docs.microsoft.com/intune/device-locate)</span><span class="sxs-lookup"><span data-stu-id="97025-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="97025-110">**GYIK**</span><span class="sxs-lookup"><span data-stu-id="97025-110">**FAQ**</span></span>

<span data-ttu-id="97025-111">K: Távoli műveletet adtam ki a vállalati adatok eszközről való eltávolítására, és most függőállapotban ragadt.</span><span class="sxs-lookup"><span data-stu-id="97025-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="97025-112">Válasz: Ahhoz, hogy egy távoli művelet sikeresen befejeződjen, a megcélzott eszköznek online és kifogástalan állapotúnak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="97025-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="97025-113">A következő esetekben a távoli művelet 30 napig függőállapotban marad, vagy amíg az eszköz nem nyugtázza a parancsot:</span><span class="sxs-lookup"><span data-stu-id="97025-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="97025-114">Ha az eszköz nem rendelkezik kapcsolattal</span><span class="sxs-lookup"><span data-stu-id="97025-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="97025-115">Amikor az eszköz elveszíti felügyeleti állapotát az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="97025-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="97025-116">Ha úgy gondolja, hogy egy eszköz már nem jelentkezik be, és nem tudja eltávolítani a vállalati adatokat, válassza a Törlés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="97025-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="97025-117">A törlés eltávolítja az eszközrekordot, így az már nem jelenik meg az Intune eszközök listájában.</span><span class="sxs-lookup"><span data-stu-id="97025-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="97025-118">Ha az eszköz ismét aktívvá válik, a felhasználónak újra regisztrálnia kell azt.</span><span class="sxs-lookup"><span data-stu-id="97025-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="97025-119">K: Miért nem érhetők el bizonyos távoli műveletek?</span><span class="sxs-lookup"><span data-stu-id="97025-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="97025-120">A: Nem minden platform támogatja az összes távoli eszközműveletet.</span><span class="sxs-lookup"><span data-stu-id="97025-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="97025-121">A következő távoli műveletek platformspecifikusak, így csak a megjegyzett platformokhoz érhetők el.</span><span class="sxs-lookup"><span data-stu-id="97025-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="97025-122">Az aktiválási zár megkerülése (csak iOS)</span><span class="sxs-lookup"><span data-stu-id="97025-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="97025-123">Új kezdet (csak Windows)</span><span class="sxs-lookup"><span data-stu-id="97025-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="97025-124">Elveszett mód (csak iOS esetén)</span><span class="sxs-lookup"><span data-stu-id="97025-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="97025-125">Az eszköz megkeresése (csak iOS esetén)</span><span class="sxs-lookup"><span data-stu-id="97025-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="97025-126">Újraindítás (csak Windows)</span><span class="sxs-lookup"><span data-stu-id="97025-126">Restart (Windows only)</span></span>

<span data-ttu-id="97025-127">Az egyes műveletekről további információt az [Elérhető eszközműveletek (Available device actions) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszköz](https://docs.microsoft.com/intune/device-management#available-device-actions)</span><span class="sxs-lookup"><span data-stu-id="97025-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>