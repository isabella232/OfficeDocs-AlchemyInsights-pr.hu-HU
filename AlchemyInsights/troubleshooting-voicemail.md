---
title: 'A hangposta hibaelhárítása '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677964"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="af9a5-102">A hangposta hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="af9a5-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="af9a5-103">Ügyeljen arra, hogy a foglalt elfoglalt funkció a szándékos legyen.</span><span class="sxs-lookup"><span data-stu-id="af9a5-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="af9a5-104">Ha ez a funkció nem szükséges a felhasználónál:</span><span class="sxs-lookup"><span data-stu-id="af9a5-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="af9a5-105">Nyissa meg a [Teams felügyeleti központot](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="af9a5-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="af9a5-106">A bal oldali sínre való **navigáláshoz** a  >  **hanghívási házirendek**  >  **kezelése** a **hívási házirendben**.</span><span class="sxs-lookup"><span data-stu-id="af9a5-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="af9a5-107">Válassza a **felhasználók kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="af9a5-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="af9a5-108">A **híváskor** a felhasználó keresése és a hívási házirend módosítása egy olyanra, amely **elfoglalt állapotban van.**</span><span class="sxs-lookup"><span data-stu-id="af9a5-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="af9a5-109">Kattintson az **Alkalmaz** gombra.</span><span class="sxs-lookup"><span data-stu-id="af9a5-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="af9a5-110">A házirendek módosításai akár 24 órát is igénybe vehetik a replikálást.</span><span class="sxs-lookup"><span data-stu-id="af9a5-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="af9a5-111">A funkcióról a következő témakörben olvashat bővebben: a foglalt [on elfoglalt funkció a hívás közben is elérhető](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="af9a5-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
