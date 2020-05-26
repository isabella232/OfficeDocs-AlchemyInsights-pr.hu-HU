---
title: 618 Naptármegosztási szabályzat
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373001"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="984d7-102">Házirendhiba naptár megosztásakor</span><span class="sxs-lookup"><span data-stu-id="984d7-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="984d7-103">Az adott helyzetnek megfelelően tegye a következők egyikét:</span><span class="sxs-lookup"><span data-stu-id="984d7-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="984d7-104">Csatlakozzon az Exchange Online-hoz a Távoli PowerShell használatával.</span><span class="sxs-lookup"><span data-stu-id="984d7-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="984d7-105">További információt a [Csatlakozás az Exchange Online-hoz távoli PowerShell használatával című](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="984d7-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="984d7-106">A helyszíni kiszolgálón nyissa meg az Exchange Management Shell t.</span><span class="sxs-lookup"><span data-stu-id="984d7-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="984d7-107">Határozza meg a felhasználóhoz rendelt megosztási házirendet.</span><span class="sxs-lookup"><span data-stu-id="984d7-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="984d7-108">Ehhez futtassa a következő parancsot, és vegye figyelembe a visszaadott házirendet:</span><span class="sxs-lookup"><span data-stu-id="984d7-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="984d7-109">Frissítse a felhasználó megosztási házirendjeit.</span><span class="sxs-lookup"><span data-stu-id="984d7-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="984d7-110">Ehhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="984d7-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="984d7-111">Nyissa meg az Exchange Felügyeleti központot.</span><span class="sxs-lookup"><span data-stu-id="984d7-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="984d7-112">Kattintson a **Szervezet**elemre, majd kattintson duplán arra a házirendre, amely az Egyéni megosztás csoportban van a felhasználóhoz **rendelve.**</span><span class="sxs-lookup"><span data-stu-id="984d7-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="984d7-113">Ez az a házirend, amelyet a 2.</span><span class="sxs-lookup"><span data-stu-id="984d7-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="984d7-114">A Megosztási szabály lapon jelölje ki a megosztani kívánt **adatok megadása**csoportban az engedélyezni kívánt naptármegosztási szintet. kattintson a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="984d7-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="984d7-115">További információ: ["A házirend nem engedélyezi az engedélyek megadását ezen a szinten egy vagy több címzett(ek)nek" hibaüzenet jelenik](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)meg, amikor a felhasználó megpróbálja megosztani a naptárat.</span><span class="sxs-lookup"><span data-stu-id="984d7-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
