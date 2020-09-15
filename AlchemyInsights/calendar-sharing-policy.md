---
title: 618 naptár-megosztási házirend
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684232"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="07c0f-102">Házirend-hiba a naptár megosztásakor</span><span class="sxs-lookup"><span data-stu-id="07c0f-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="07c0f-103">A helyzetnek megfelelően végezze el az alábbi műveletek egyikét:</span><span class="sxs-lookup"><span data-stu-id="07c0f-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="07c0f-104">Csatlakozás az Exchange Online-hoz távoli PowerShell használatával.</span><span class="sxs-lookup"><span data-stu-id="07c0f-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="07c0f-105">További információt a [Csatlakozás az Exchange Online-hoz távoli PowerShell használatával](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="07c0f-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="07c0f-106">Nyissa meg az Exchange Management shellt a helyszíni kiszolgálón.</span><span class="sxs-lookup"><span data-stu-id="07c0f-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="07c0f-107">Határozza meg a felhasználóhoz rendelt megosztási házirendet.</span><span class="sxs-lookup"><span data-stu-id="07c0f-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="07c0f-108">Ehhez futtassa a következő parancsot, és jegyezze fel a visszaadott házirendet:</span><span class="sxs-lookup"><span data-stu-id="07c0f-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="07c0f-109">A felhasználó megosztási házirendjének frissítése</span><span class="sxs-lookup"><span data-stu-id="07c0f-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="07c0f-110">Ehhez hajtsa végre a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="07c0f-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="07c0f-111">Nyissa meg az Exchange felügyeleti központot.</span><span class="sxs-lookup"><span data-stu-id="07c0f-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="07c0f-112">Kattintson a **szervezet**elemre, majd kattintson duplán arra a házirendre, amely az **Egyéni megosztás**csoportban van hozzárendelve a felhasználóhoz.</span><span class="sxs-lookup"><span data-stu-id="07c0f-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="07c0f-113">Ez a házirend, amely a 2. lépésben tért vissza.</span><span class="sxs-lookup"><span data-stu-id="07c0f-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="07c0f-114">A megosztási szabály lapon válassza ki az engedélyezni kívánt naptár megosztási szintjét az **adja meg, hogy milyen információkat szeretne megosztani**; kattintson a **Mentés**gombra.</span><span class="sxs-lookup"><span data-stu-id="07c0f-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="07c0f-115">További információt a következő témakörben talál: ["a házirend nem engedélyezi az engedélyeket a címzett (ek) nek egy vagy több címzett számára" hibaüzenet jelenik meg, amikor a felhasználó megpróbálja megosztani a naptárat](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="07c0f-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
