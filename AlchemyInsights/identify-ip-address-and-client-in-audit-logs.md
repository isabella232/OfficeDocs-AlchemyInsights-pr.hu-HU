---
title: IP-cím és a naplókat az ügyfél azonosítása
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909303"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="b1580-102">IP-cím és a naplókat az ügyfél azonosítása</span><span class="sxs-lookup"><span data-stu-id="b1580-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="b1580-103">Az IP-cím, amely megfelel egy tevékenység egy felhasználó vagy rendszergazda által a naplófájlban jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="b1580-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="b1580-104">Az ügyfél adatait is naplózza.</span><span class="sxs-lookup"><span data-stu-id="b1580-104">The client information is also logged.</span></span> <span data-ttu-id="b1580-105">Az alábbiakban a lépéseket, hogy ilyen információk azonosítása</span><span class="sxs-lookup"><span data-stu-id="b1580-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="b1580-106">Jelentkezzen be az [Office 365 biztonsági & kompatibilitási központ](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b1580-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b1580-107">Kattintson a **Keresés és a vizsgálat** , és válassza a **Könyvvizsgálati napló Search**.</span><span class="sxs-lookup"><span data-stu-id="b1580-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="b1580-108">Ha érdekli az adott tevékenység, **tevékenységek** listából jelölje ki azt.</span><span class="sxs-lookup"><span data-stu-id="b1580-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="b1580-109">Ha nem, minden tevékenység visszatér a kijelölt felhasználó (alapértelmezett beállítás).</span><span class="sxs-lookup"><span data-stu-id="b1580-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="b1580-110">**Megjegyzés**: egyes tevékenységek nem áll rendelkezésre a **tevékenységek** menü; azonban e könyvvizsgálati elemek **Minden tevékenységek eredményének megjelenítése** a kijelölt (alapértelmezett beállítás) esetén visszatér.</span><span class="sxs-lookup"><span data-stu-id="b1580-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="b1580-111">A **felhasználók** mezőben adja meg a felhasználónevet, válassza ki a megfelelő dátumtartományt a tevékenység, és kattintson a **Keresés**.</span><span class="sxs-lookup"><span data-stu-id="b1580-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="b1580-112">Az eredmények a tevékenység az eredmények ablaktáblájában az IP-cím látható.</span><span class="sxs-lookup"><span data-stu-id="b1580-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="b1580-113">Válassza ki az elemzési rekord részletes információt a **Részletek** úszó (például ügyfél, felhasználó által végzett művelet, stb.).</span><span class="sxs-lookup"><span data-stu-id="b1580-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="b1580-114">További tudnivalókért tanulmányozza [a feltört fiók elérésére használt számítógép IP-cím megkeresése](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="b1580-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
