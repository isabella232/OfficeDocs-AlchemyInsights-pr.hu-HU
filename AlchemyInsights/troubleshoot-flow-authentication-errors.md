---
title: Adatfolyam-hitelesítési hibák – problémamegoldás
ms.author: pebaum
author: pebaum
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3d49d15d243dd98afc6f78b9e75f0cfa74c2cd7c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050635"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="bbd3f-102">Adatfolyam-hitelesítési hibák – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="bbd3f-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="bbd3f-103">Sok esetben a sikertelen tranzakciók a hitelesítési hiba miatt meghiúsulnak.</span><span class="sxs-lookup"><span data-stu-id="bbd3f-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="bbd3f-104">Ha ilyen típusú hibát tartalmaz, a hibaüzenet "nem engedélyezett", illetve 401-es vagy 403-es hibakódot jelenít meg.</span><span class="sxs-lookup"><span data-stu-id="bbd3f-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="bbd3f-105">A hitelesítési hibát általában a következő kapcsolat frissítésével lehet kijavítani:</span><span class="sxs-lookup"><span data-stu-id="bbd3f-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="bbd3f-106">A webportál tetején kattintson vagy érintse meg a fogaskerék ikont a beállítások menü megnyitásához, majd kattintson vagy koppintson a **kapcsolatok**elemre.</span><span class="sxs-lookup"><span data-stu-id="bbd3f-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="bbd3f-107">Görgessen arra a kapcsolatra, amelynek a jogosulatlan hibüzenetét látta.</span><span class="sxs-lookup"><span data-stu-id="bbd3f-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="bbd3f-108">A kapcsolat mellett kattintson vagy koppintson a **jelszó ellenőrzése** hivatkozásra az üzenetben arról a kapcsolatról, amely nincs hitelesítve.</span><span class="sxs-lookup"><span data-stu-id="bbd3f-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="bbd3f-109">A megjelenő utasításokat követve ellenőrizze a hitelesítő adatait, térjen vissza az adatfolyam-futtatási hibának, majd kattintson az **ismételt küldés**gombra, és koppintson rá.</span><span class="sxs-lookup"><span data-stu-id="bbd3f-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="bbd3f-110">További segítségért olvassa el az [adatfolyam hibaelhárítása](https://go.microsoft.com/fwlink/?linkid=872110)című témakört.</span><span class="sxs-lookup"><span data-stu-id="bbd3f-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

