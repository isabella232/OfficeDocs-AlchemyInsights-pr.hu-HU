---
title: Ip-cím és ügyfél azonosítása a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716390"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="bba61-102">Ip-cím és ügyfél azonosítása a naplókban</span><span class="sxs-lookup"><span data-stu-id="bba61-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="bba61-103">A Microsoft 365-felhasználó vagy -rendszergazda tevékenységének megfelelő IP-cím a naplókban jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="bba61-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="bba61-104">Az ügyféladatok is naplózva lesznek.</span><span class="sxs-lookup"><span data-stu-id="bba61-104">The client information is also logged.</span></span> <span data-ttu-id="bba61-105">Az alábbi lépésekkel azonosíthatók az ilyen információk</span><span class="sxs-lookup"><span data-stu-id="bba61-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="bba61-106">Jelentkezzen be a [Microsoft 365 Biztonsági & megfelelőségi központjába.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="bba61-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="bba61-107">Nyissa meg a **Keresési** > **napló keresési naplójának keresési** lapját.</span><span class="sxs-lookup"><span data-stu-id="bba61-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="bba61-108">Ha érdekel egy adott tevékenység, válassza ki a **Tevékenységek** listából.</span><span class="sxs-lookup"><span data-stu-id="bba61-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="bba61-109">Ha nem, akkor a kijelölt felhasználó minden tevékenysége visszakerül (alapértelmezett beállítás).</span><span class="sxs-lookup"><span data-stu-id="bba61-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="bba61-110">**Megjegyzés**: Előfordulhat, hogy bizonyos tevékenységek nem érhetők el a **Tevékenységek** menüben; ezek a naplózási elemek azonban akkor kerülnek visszaadásra, ha **az összes tevékenység eredményének megjelenítése** be van jelölve (alapértelmezett beállítás).</span><span class="sxs-lookup"><span data-stu-id="bba61-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="bba61-111">Adja meg a felhasználónevet a **Felhasználók** mezőben, válassza ki a tevékenységhez megfelelő dátumtartományt, majd kattintson a **Keresés gombra.**</span><span class="sxs-lookup"><span data-stu-id="bba61-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="bba61-112">Az eredményekben az adott tevékenység IP-címét láthatja az eredmények ablaktáblában.</span><span class="sxs-lookup"><span data-stu-id="bba61-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="bba61-113">Válassza ki a naplózási rekordot a **Részletek** úszó panelrészletes információinak megtekintéséhez (például Ügyfél, Műveletet végző felhasználó stb.).</span><span class="sxs-lookup"><span data-stu-id="bba61-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="bba61-114">További információt [a feltört fiók eléréséhez használt számítógép IP-címének megkeresése](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="bba61-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
