---
title: Folyamat hitelesítési hibák elhárítása
ms.author: kaarins
author: kaarins
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: fbb2ea4f0c6e582dae71371d958667162a138346
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293758"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="f5032-102">Folyamat hitelesítési hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="f5032-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="f5032-p101">Sok esetben a forgalom hitelesítési hiba miatt sikertelen. Ha ilyen típusú hiba, a hibaüzenet tartalmazza "Nem engedélyezett", vagy egy 401 vagy 403 hibakód jelenik meg. Hitelesítési hiba történt a kapcsolat frissítése általában megoldásához:</span><span class="sxs-lookup"><span data-stu-id="f5032-p101">In many cases, flows fail because of an authentication error. If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears. You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="f5032-106">A webportál tetején kattintson vagy koppintson a sebességváltó ikonra kattintva nyissa meg a beállítások menüt, majd kattintson vagy koppintson a **kapcsolatok**.</span><span class="sxs-lookup"><span data-stu-id="f5032-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="f5032-107">Görgessen a kapcsolatra, amelyhez a jogosulatlan hibaüzenet látta.</span><span class="sxs-lookup"><span data-stu-id="f5032-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="f5032-108">A kapcsolat mellett kattintson vagy koppintson a **jelszó megerősítése** az üzenet nincs hitelesítve a kapcsolat hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="f5032-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="f5032-109">A hitelesítő adatok ellenőrzéséhez, hogy jelennek meg, térjen vissza a folyamat indításakor hiba, majd kattintson vagy koppintson a **küldje el újra**az utasításokat követve.</span><span class="sxs-lookup"><span data-stu-id="f5032-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="f5032-110">További segítséget talál a [hibaelhárítási folyamat](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="f5032-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

