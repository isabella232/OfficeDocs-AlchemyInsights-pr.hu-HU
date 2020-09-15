---
title: Az IP-cím és az ügyfél meghatározása a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668312"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="2f971-102">Az IP-cím és az ügyfél meghatározása a naplókban</span><span class="sxs-lookup"><span data-stu-id="2f971-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="2f971-103">A Microsoft 365-felhasználók vagy-rendszergazdák által egy tevékenységhez tartozó IP-cím megjelenik a naplókban.</span><span class="sxs-lookup"><span data-stu-id="2f971-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="2f971-104">Az ügyfél adatai is naplózásra kerülnek.</span><span class="sxs-lookup"><span data-stu-id="2f971-104">The client information is also logged.</span></span> <span data-ttu-id="2f971-105">Az alábbi lépésekkel azonosíthatja ezeket az információkat</span><span class="sxs-lookup"><span data-stu-id="2f971-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="2f971-106">Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="2f971-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2f971-107">Nyissa meg a **keresési**  >  **napló keresési** lapját.</span><span class="sxs-lookup"><span data-stu-id="2f971-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="2f971-108">Ha egy adott tevékenység érdekli, jelölje ki a **tevékenységek** listából.</span><span class="sxs-lookup"><span data-stu-id="2f971-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="2f971-109">Ha nem, a program az összes tevékenységet visszaadja a kijelölt felhasználónak (alapértelmezett beállítás).</span><span class="sxs-lookup"><span data-stu-id="2f971-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="2f971-110">**Megjegyzés**: Előfordulhat, hogy bizonyos tevékenységek nem érhetők el a **tevékenységek** menüben; Ha azonban az **összes tevékenység eredményének megjelenítése** jelölőnégyzet be van jelölve, akkor a rendszer ezeket a naplózási elemeket adja vissza (alapértelmezett beállítás).</span><span class="sxs-lookup"><span data-stu-id="2f971-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="2f971-111">Adja meg a felhasználónevet a **felhasználók** mezőben, válassza ki a tevékenységhez megfelelő dátumtartományt, majd kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="2f971-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="2f971-112">A találatok között láthatja az adott tevékenységhez tartozó IP-címet az eredmények munkaablakban.</span><span class="sxs-lookup"><span data-stu-id="2f971-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="2f971-113">Válassza a könyvvizsgálati rekordot, ha részletes információkat szeretne látni a részletek (például ügyfél, felhasználó, művelet stb.) **részleteiről** .</span><span class="sxs-lookup"><span data-stu-id="2f971-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="2f971-114">További információért olvassa el a [sérült fiók eléréséhez használt számítógép IP-címének megkeresése](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)című témakört.</span><span class="sxs-lookup"><span data-stu-id="2f971-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
