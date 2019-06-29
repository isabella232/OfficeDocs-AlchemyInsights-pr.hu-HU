---
title: Beérkezett üzenetek szabály tevékenység naplók azonosítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383027"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="affcd-102">Beérkezett üzenetek szabály tevékenység naplók azonosítása</span><span class="sxs-lookup"><span data-stu-id="affcd-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="affcd-103">A biztonsági & Megfelelési központba ellenőrzési napló keresés segítségével megtekinteni a Beérkezett üzenetek szabály eseményeket (létrehozása, módosítása és törlése a Beérkezett üzenetekre vonatkozó szabályok).</span><span class="sxs-lookup"><span data-stu-id="affcd-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="affcd-104">Jelentkezzen be az [Office 365 biztonsági & kompatibilitási központ](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="affcd-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="affcd-105">Kattintson a **Keresés és a vizsgálat** , és válassza a **Könyvvizsgálati napló Search**.</span><span class="sxs-lookup"><span data-stu-id="affcd-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="affcd-106">Jelöljük ki a dátumot a **Kezdő dátum** és **Záró dátum** mezőket.</span><span class="sxs-lookup"><span data-stu-id="affcd-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="affcd-107">**Exchange postaláda tevékenységek**területen ellenőrizze a **tevékenységeket** a mező értéke **Új-InboxRule létrehozása/módosítása/engedélyezése/letiltása a Beérkezett üzenetek szabály**.</span><span class="sxs-lookup"><span data-stu-id="affcd-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="affcd-108">Kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="affcd-108">Click **Search**.</span></span>

<span data-ttu-id="affcd-109">Az eredmények a válassza ki a tételt generál.</span><span class="sxs-lookup"><span data-stu-id="affcd-109">In the results, select an audit record.</span></span> <span data-ttu-id="affcd-110">Kattintson a részletek úszó **További információ**.</span><span class="sxs-lookup"><span data-stu-id="affcd-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="affcd-111">A Beérkezett üzenetek Szabálybeállítások információt a **Paraméterek** mezőben jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="affcd-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="affcd-112">További tudnivalókért tanulmányozza a [meghatározása, ha az Üzenetfájl-szabályt létrehozó felhasználó](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="affcd-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
