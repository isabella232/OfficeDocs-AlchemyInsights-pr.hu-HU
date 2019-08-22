---
title: IP-cím és a naplókat az ügyfél azonosítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539031"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="0b4e6-102">IP-cím és a naplókat az ügyfél azonosítása</span><span class="sxs-lookup"><span data-stu-id="0b4e6-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="0b4e6-103">Az IP-cím, amely megfelel az Office 365-felhasználó vagy rendszergazda által tevékenység jelenik meg a naplókat.</span><span class="sxs-lookup"><span data-stu-id="0b4e6-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="0b4e6-104">Az ügyfél adatait is naplózza.</span><span class="sxs-lookup"><span data-stu-id="0b4e6-104">The client information is also logged.</span></span> <span data-ttu-id="0b4e6-105">Az alábbiakban a lépéseket, hogy ilyen információk azonosítása</span><span class="sxs-lookup"><span data-stu-id="0b4e6-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="0b4e6-106">Jelentkezzen be az [Office 365 biztonsági & Megfelelési központba](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="0b4e6-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="0b4e6-107">Keresse fel a **keresési** > **Audit napló** keresőlap.</span><span class="sxs-lookup"><span data-stu-id="0b4e6-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="0b4e6-108">Ha érdekli az adott tevékenység, **tevékenységek** listából jelölje ki azt.</span><span class="sxs-lookup"><span data-stu-id="0b4e6-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="0b4e6-109">Ha nem, minden tevékenység visszatér a kijelölt felhasználó (alapértelmezett beállítás).</span><span class="sxs-lookup"><span data-stu-id="0b4e6-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="0b4e6-110">**Megjegyzés**: egyes tevékenységek nem áll rendelkezésre a **tevékenységek** menü; azonban e könyvvizsgálati elemek **Minden tevékenységek eredményének megjelenítése** a kijelölt (alapértelmezett beállítás) esetén visszatér.</span><span class="sxs-lookup"><span data-stu-id="0b4e6-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="0b4e6-111">A **felhasználók** mezőben adja meg a felhasználónevet, válassza ki a megfelelő dátumtartományt a tevékenység, és kattintson a **Keresés**.</span><span class="sxs-lookup"><span data-stu-id="0b4e6-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="0b4e6-112">Az eredmények a tevékenység az eredmények ablaktáblájában az IP-cím látható.</span><span class="sxs-lookup"><span data-stu-id="0b4e6-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="0b4e6-113">Válassza ki az elemzési rekord részletes információt a **Részletek** úszó (például ügyfél, felhasználó által végzett művelet, stb.).</span><span class="sxs-lookup"><span data-stu-id="0b4e6-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="0b4e6-114">További tudnivalókért tanulmányozza [a feltört fiók elérésére használt számítógép IP-cím megkeresése](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="0b4e6-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
