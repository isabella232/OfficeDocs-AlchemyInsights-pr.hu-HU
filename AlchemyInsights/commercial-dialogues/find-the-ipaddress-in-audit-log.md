---
title: Az IP-cím megkeresés a naplóban
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482608"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="ed492-102">Az IP-cím megkeresés a naplóban</span><span class="sxs-lookup"><span data-stu-id="ed492-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="ed492-103">A naplókban megjelenik a felhasználó vagy rendszergazda által végrehajtott tevékenység IP-címe.</span><span class="sxs-lookup"><span data-stu-id="ed492-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="ed492-104">Az ügyféladatokat is naplózza a rendszer.</span><span class="sxs-lookup"><span data-stu-id="ed492-104">The client information is also logged.</span></span> <span data-ttu-id="ed492-105">Így azonosíthatja az IP-címet:</span><span class="sxs-lookup"><span data-stu-id="ed492-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="ed492-106">Menjen az [Office 365 Biztonsági & megfelelőségi központba.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="ed492-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ed492-107">Válassza **a Keresés**  >  **[naplókeresés lehetőséget.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="ed492-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ed492-108">Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, akkor most kapcsolja be.</span><span class="sxs-lookup"><span data-stu-id="ed492-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ed492-109">Ha ez a funkció nincs engedélyezve, a keresési eredmények nem fogják tudni lekeresni az adatokat a korábbi dátumok alapján.</span><span class="sxs-lookup"><span data-stu-id="ed492-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ed492-110">Ha egy adott tevékenységre kíváncsi, válassza ki azt a Tevékenységek **listából;** ellenkező esetben a rendszer alapértelmezés szerint az összes tevékenységet visszaadja a kijelölt felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="ed492-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="ed492-111">Előfordulhat, hogy egyes tevékenységek nem érhetők el a Tevékenységek **menüben;** ezeket a naplóelemeket azonban a program akkor is visszaadja, ha az összes tevékenység eredményének **megjelenítése** (alapértelmezett beállítás) van bejelölve.</span><span class="sxs-lookup"><span data-stu-id="ed492-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="ed492-112">Adja meg a dátumtartományt, és a **Felhasználók** mezőben válassza ki a vizsgálni kívánt felhasználó felhasználónevét.</span><span class="sxs-lookup"><span data-stu-id="ed492-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="ed492-113">Válassza a **Keresés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed492-113">Select **Search**.</span></span> <span data-ttu-id="ed492-114">A tevékenységek az Eredmények **alatt jelennek meg.**</span><span class="sxs-lookup"><span data-stu-id="ed492-114">The activities appear under **Results**.</span></span> <span data-ttu-id="ed492-115">Az egyes tevékenységek IP-címét láthatja.</span><span class="sxs-lookup"><span data-stu-id="ed492-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="ed492-116">A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a **További információ lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ed492-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="ed492-117">További információért olvassa el a Keresés az [Office 365 naplójában](https://go.microsoft.com/fwlink/?linkid=2103944)a gyakori esetek elhárításához.</span><span class="sxs-lookup"><span data-stu-id="ed492-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>