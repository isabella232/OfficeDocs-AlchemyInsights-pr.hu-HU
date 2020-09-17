---
title: A beérkezett üzenetekre vonatkozó szabályok tevékenységének meghatározása a naplókban
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779053"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="861c5-102">A beérkezett üzenetekre vonatkozó szabályok tevékenységének meghatározása a naplókban</span><span class="sxs-lookup"><span data-stu-id="861c5-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="861c5-103">A beérkezett üzenetekre vonatkozó szabályok eseményei (a beérkezett üzenetekre vonatkozó szabályok létrehozása, módosítása és törlése) a Microsoft 365 biztonsági & megfelelőségi központban használhatók a naplózási naplóban.</span><span class="sxs-lookup"><span data-stu-id="861c5-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="861c5-104">Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="861c5-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="861c5-105">Nyissa meg a **keresési**  >  **napló keresési** lapját.</span><span class="sxs-lookup"><span data-stu-id="861c5-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="861c5-106">Válassza ki a dátumtartomány értékét a **kezdési dátum** és a **Záró dátum** mezőben.</span><span class="sxs-lookup"><span data-stu-id="861c5-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="861c5-107">Az **Exchange-postaláda tevékenységei**területen ellenőrizze, hogy a **tevékenységek** mező be van-e állítva: **új – a InboxRule létrehozása/módosítása/engedélyezése/letiltása a levelezési szabály letiltásával**.</span><span class="sxs-lookup"><span data-stu-id="861c5-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="861c5-108">Kattintson a **Keresés**gombra.</span><span class="sxs-lookup"><span data-stu-id="861c5-108">Click **Search**.</span></span>

<span data-ttu-id="861c5-109">A találatok között válasszon egy naplózási rekordot.</span><span class="sxs-lookup"><span data-stu-id="861c5-109">In the results, select an audit record.</span></span> <span data-ttu-id="861c5-110">Kattintson a részletek menü **További információk**parancsára.</span><span class="sxs-lookup"><span data-stu-id="861c5-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="861c5-111">A beérkezett üzenetekre vonatkozó szabály beállításairól szóló információk a **Parameters (paraméterek** ) mezőben láthatók.</span><span class="sxs-lookup"><span data-stu-id="861c5-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="861c5-112">További információ: [a Beérkezett üzenetek szabályát létrehozó felhasználó létrehozása](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="861c5-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
