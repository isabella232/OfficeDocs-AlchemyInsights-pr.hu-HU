---
title: A beérkezett üzenetek szabályának tevékenységének azonosítása a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716426"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="f20ec-102">A beérkezett üzenetek szabályának tevékenységének azonosítása a naplókban</span><span class="sxs-lookup"><span data-stu-id="f20ec-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="f20ec-103">A Microsoft 365 Biztonsági & megfelelőségi központban végzett naplókeresés sel megtekintheti a beérkezett üzenetekre vonatkozó szabályok eseményeit (a beérkezett üzenetekre vonatkozó szabályok létrehozása, módosítása és törlése).</span><span class="sxs-lookup"><span data-stu-id="f20ec-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="f20ec-104">Jelentkezzen be a [Microsoft 365 Biztonsági & megfelelőségi központjába.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="f20ec-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f20ec-105">Nyissa meg a **Keresési** > **napló keresési naplójának keresési** lapját.</span><span class="sxs-lookup"><span data-stu-id="f20ec-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="f20ec-106">Válassza ki a dátumtartományt a **Kezdési dátum** és a **Záró dátum** mezőben.</span><span class="sxs-lookup"><span data-stu-id="f20ec-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="f20ec-107">Az **Exchange-postaláda-tevékenységek csoportban**ellenőrizze, hogy a **Tevékenységek** mező új **beérkezett üzenetekre vonatkozó létrehozási/módosítási/enable/disable beérkezett üzenetekre vonatkozó szabály értékre van-e állítva.**</span><span class="sxs-lookup"><span data-stu-id="f20ec-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="f20ec-108">Kattintson a **Keresés gombra.**</span><span class="sxs-lookup"><span data-stu-id="f20ec-108">Click **Search**.</span></span>

<span data-ttu-id="f20ec-109">Az eredmények között jelöljön ki egy naplózási rekordot.</span><span class="sxs-lookup"><span data-stu-id="f20ec-109">In the results, select an audit record.</span></span> <span data-ttu-id="f20ec-110">A részletes úszó panelen kattintson a **További információ gombra.**</span><span class="sxs-lookup"><span data-stu-id="f20ec-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f20ec-111">A beérkezett üzenetek szabálybeállításaival kapcsolatos információk a **Paraméterek** mezőben jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="f20ec-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="f20ec-112">További [információ: Annak meghatározása, hogy a felhasználó létrehozott-e beérkezett üzenetekre vonatkozó szabályt.](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="f20ec-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
