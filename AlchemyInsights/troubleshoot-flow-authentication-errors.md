---
title: Folyamatalapú hitelesítési hibák elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 70451f074a65a4454faeadd188a31783be8e6c7e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759730"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="7cd3a-102">Folyamatalapú hitelesítési hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="7cd3a-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="7cd3a-103">Sok esetben a folyamatok hitelesítési hiba miatt sikertelenek.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="7cd3a-104">Ha ilyen típusú hiba történik, a hibaüzenet "Jogosulatlan" üzenetet tartalmaz, vagy egy 401-es vagy 403-as hibakódot.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="7cd3a-105">A hitelesítési hibákat általában a kapcsolat frissítésével javíthatja ki:</span><span class="sxs-lookup"><span data-stu-id="7cd3a-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="7cd3a-106">A webportál tetején kattintson vagy koppintson a fogaskerék ikonra a Beállítások menü megnyitásához, majd a **Kapcsolatok**parancsra.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="7cd3a-107">Görgessen ahhoz a kapcsolathoz, amelyhez a Jogosulatlan hibaüzenet et látta.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="7cd3a-108">A kapcsolat mellett kattintson vagy koppintson a **Jelszó ellenőrzése** hivatkozásra az üzenetben arról, hogy a kapcsolat nincs hitelesítve.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="7cd3a-109">Ellenőrizze hitelesítő adatait a megjelenő utasításokat követve, térjen vissza a folyamatfuttatási hibához, majd kattintson vagy koppintson az **Újraküldés gombra.**</span><span class="sxs-lookup"><span data-stu-id="7cd3a-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="7cd3a-110">További segítséget a [Folyamat hibaelhárítása című témakörben talál.](https://go.microsoft.com/fwlink/?linkid=872110)</span><span class="sxs-lookup"><span data-stu-id="7cd3a-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

