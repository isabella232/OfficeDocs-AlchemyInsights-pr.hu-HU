---
title: Tudja meg, hogy ki állíthatja be az továbbítást a postaládában, és hogyan
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482299"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="c980c-102">Tudja meg, hogy ki állíthatja be az továbbítást a postaládában, és hogyan</span><span class="sxs-lookup"><span data-stu-id="c980c-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="c980c-103">Ha a külső továbbítás be van állítva egy postaládában, a tevékenység a Set-Mailbox részeként lesz naplózásra.</span><span class="sxs-lookup"><span data-stu-id="c980c-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="c980c-104">Így találhatja meg a tevékenységet a naplóban:</span><span class="sxs-lookup"><span data-stu-id="c980c-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="c980c-105">Menjen az [Office 365 Biztonsági & megfelelőségi központba.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="c980c-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="c980c-106">Válassza **a Keresés** >  **naplókeresés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c980c-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="c980c-107">Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, akkor most kapcsolja be.</span><span class="sxs-lookup"><span data-stu-id="c980c-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="c980c-108">Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem fogják tudni lekeresni az előző dátumok adatait.</span><span class="sxs-lookup"><span data-stu-id="c980c-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="c980c-109">Győződjön meg arról, **hogy a Tevékenységek** mezőben az összes tevékenység eredményének megjelenítése (az alapértelmezett beállítás) van megjelölve. </span><span class="sxs-lookup"><span data-stu-id="c980c-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="c980c-110">Adja meg a dátumtartományt.</span><span class="sxs-lookup"><span data-stu-id="c980c-110">Specify the date range.</span></span> <span data-ttu-id="c980c-111">Nem kell megadnia a felhasználónevet.</span><span class="sxs-lookup"><span data-stu-id="c980c-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="c980c-112">Válassza a **Keresés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c980c-112">Select **Search**.</span></span> <span data-ttu-id="c980c-113">A tevékenységek az Eredmények **alatt jelennek meg.**</span><span class="sxs-lookup"><span data-stu-id="c980c-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="c980c-114">Válassza **az Eredmények szűrése** lehetőséget, majd írja be a **Set-mailbox** mezőt a **Tevékenységszűrő** mezőbe.</span><span class="sxs-lookup"><span data-stu-id="c980c-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="c980c-115">Ez az összes **Set-Mailbox-tevékenységet visszaadja.**</span><span class="sxs-lookup"><span data-stu-id="c980c-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="c980c-116">A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a **További információ lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c980c-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="c980c-117">A **Paraméterek alatt** láthatja a postaládában beállított továbbítási e-mail-címet.</span><span class="sxs-lookup"><span data-stu-id="c980c-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="c980c-118">A **UserID** az a felhasználó, aki külső továbbítást beállított a postaládában.</span><span class="sxs-lookup"><span data-stu-id="c980c-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="c980c-119">További információért olvassa el a Keresés az [Office 365 naplójában](https://go.microsoft.com/fwlink/?linkid=2103944)a gyakori esetek elhárításához.</span><span class="sxs-lookup"><span data-stu-id="c980c-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>