---
title: Az aktiválási zár megkerülése felügyelt iOS-eszközökön az Intune-nal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423732"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="f6f58-102">Az aktiválási zár megkerülése felügyelt iOS-eszközökön az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="f6f58-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="f6f58-103">Az iOS-eszközök aktiválási zárjának megkerülésének lehetősége megkönnyíti a helyreállítást abból a forgatókönyvből, amikor a felhasználó engedélyezi az aktiválási zárat egy vállalati eszközön, majd elhagyja a vállalatot.</span><span class="sxs-lookup"><span data-stu-id="f6f58-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="f6f58-104">Az aktiválási zár megkerüléséhez szükséges előfeltételek a következők:</span><span class="sxs-lookup"><span data-stu-id="f6f58-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="f6f58-105">Az eszköz az, hogy a "felügyelt".</span><span class="sxs-lookup"><span data-stu-id="f6f58-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="f6f58-106">Az aktiválási zárolás sikeresen engedélyezve van az Intune iOS-eszközkorlátozási házirendjével.</span><span class="sxs-lookup"><span data-stu-id="f6f58-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="f6f58-107">Ezenkívül az aktiválási zár megkerülésekénél a következőket kell tennie:</span><span class="sxs-lookup"><span data-stu-id="f6f58-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="f6f58-108">Fizikailag birtokolják a letörölt eszközt.</span><span class="sxs-lookup"><span data-stu-id="f6f58-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="f6f58-109">Másolja a kódot, mielőtt kiadja a törlést.</span><span class="sxs-lookup"><span data-stu-id="f6f58-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="f6f58-110">**Megjegyzés:** A törlési kód nem érzékeny a kis- és nagybetűkre, ezért a "-" karakterek nem szükségesek.</span><span class="sxs-lookup"><span data-stu-id="f6f58-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="f6f58-111">További információt az [Aktiválási zár megkerülése felügyelt iOS-eszközökön az Intune-nal.](https://docs.microsoft.com/intune/device-activation-lock-bypass)</span><span class="sxs-lookup"><span data-stu-id="f6f58-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="f6f58-112">**GYIK**</span><span class="sxs-lookup"><span data-stu-id="f6f58-112">**FAQ**</span></span>

<span data-ttu-id="f6f58-113">K: **Távoli műveletet adtam ki a vállalati adatok eszközről való eltávolítására, és most függőállapotban ragadt.**</span><span class="sxs-lookup"><span data-stu-id="f6f58-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="f6f58-114">Válasz: Ahhoz, hogy egy távoli művelet sikeresen befejeződjen, a megcélzott eszköznek online és kifogástalan állapotúnak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="f6f58-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="f6f58-115">A következő esetekben a távoli művelet 30 napig függőállapotban marad, vagy amíg az eszköz nem nyugtázza a parancsot, amikor az eszköz:</span><span class="sxs-lookup"><span data-stu-id="f6f58-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="f6f58-116">Nem rendelkezik kapcsolattal.</span><span class="sxs-lookup"><span data-stu-id="f6f58-116">Does not have connectivity.</span></span>
- <span data-ttu-id="f6f58-117">Az Intune-nal elveszíti felügyeleti állapotát.</span><span class="sxs-lookup"><span data-stu-id="f6f58-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="f6f58-118">Ha úgy gondolja, hogy egy eszköz már nem jelentkezik be, és nem távolítja el a vállalati adatokat, válassza a Törlés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f6f58-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="f6f58-119">A törlés eltávolítja az eszközrekordot, így az már nem jelenik meg az Intune eszközök listájában.</span><span class="sxs-lookup"><span data-stu-id="f6f58-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="f6f58-120">Ahhoz, hogy az eszköz újra aktívvá váljon, a felhasználónak újra regisztrálnia kell az eszközt.</span><span class="sxs-lookup"><span data-stu-id="f6f58-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="f6f58-121">K: **Miért nem érhetők el bizonyos távoli műveletek?**</span><span class="sxs-lookup"><span data-stu-id="f6f58-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="f6f58-122">A: Nem minden platform támogatja az összes távoli eszközműveletet.</span><span class="sxs-lookup"><span data-stu-id="f6f58-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="f6f58-123">A következő távoli műveletek platformspecifikusak.</span><span class="sxs-lookup"><span data-stu-id="f6f58-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="f6f58-124">Az aktiválási zár megkerülése (csak iOS)</span><span class="sxs-lookup"><span data-stu-id="f6f58-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="f6f58-125">Új kezdet (csak Windows)</span><span class="sxs-lookup"><span data-stu-id="f6f58-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="f6f58-126">Elveszett mód (csak iOS esetén)</span><span class="sxs-lookup"><span data-stu-id="f6f58-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="f6f58-127">Az eszköz megkeresése (csak iOS esetén)</span><span class="sxs-lookup"><span data-stu-id="f6f58-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="f6f58-128">Újraindítás (csak Windows)</span><span class="sxs-lookup"><span data-stu-id="f6f58-128">Restart (Windows only)</span></span>

<span data-ttu-id="f6f58-129">Az egyes műveletekről további információt az [Elérhető eszközműveletek (Available device actions) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszköz](https://docs.microsoft.com/intune/device-management#available-device-actions)</span><span class="sxs-lookup"><span data-stu-id="f6f58-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>