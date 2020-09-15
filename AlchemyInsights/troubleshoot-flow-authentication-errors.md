---
title: Folyamat-hitelesítési hibák elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690569"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="644a2-102">Folyamat-hitelesítési hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="644a2-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="644a2-103">A tranzakciók sok esetben sikertelenek, mert hitelesítési hiba történt.</span><span class="sxs-lookup"><span data-stu-id="644a2-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="644a2-104">Ha ilyen típusú hibaüzenetet kap, a hibaüzenet a "nem engedélyezett" vagy az 401 vagy az 403 hibakódot tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="644a2-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="644a2-105">A kapcsolat frissítésével általában kijavíthatja a hitelesítési hibát:</span><span class="sxs-lookup"><span data-stu-id="644a2-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="644a2-106">A webes portál tetején kattintson vagy koppintson a fogaskerék ikonra a beállítások menü megnyitásához, majd kattintson vagy koppintson a **kapcsolatok**elemre.</span><span class="sxs-lookup"><span data-stu-id="644a2-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="644a2-107">Lépjen arra a kapcsolatra, amelyhez a jogosulatlan hibaüzenetet látta.</span><span class="sxs-lookup"><span data-stu-id="644a2-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="644a2-108">Kattintson vagy koppintson a kapcsolat melletti **jelszó ellenőrzése** hivatkozásra abban az üzenetben, amelyre a kapcsolat nincs hitelesítve.</span><span class="sxs-lookup"><span data-stu-id="644a2-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="644a2-109">A megjelenő utasításokat követve igazolja a hitelesítő adatait, térjen vissza az átfolyási hibára, majd kattintson vagy koppintson a **Küldés**gombra.</span><span class="sxs-lookup"><span data-stu-id="644a2-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="644a2-110">További segítségért olvassa el [a folyamat hibaelhárítása](https://go.microsoft.com/fwlink/?linkid=872110)című témakört.</span><span class="sxs-lookup"><span data-stu-id="644a2-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

