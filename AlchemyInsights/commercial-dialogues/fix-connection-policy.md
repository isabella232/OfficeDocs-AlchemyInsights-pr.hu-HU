---
title: Kapcsolati házirend kijavítás
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746750"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="d86d7-102">Kapcsolati házirend kijavítás</span><span class="sxs-lookup"><span data-stu-id="d86d7-102">Fix connection policy</span></span>

<span data-ttu-id="d86d7-103">Az e-mail biztonságosként lett megjelölve, és a felhasználó postaládájába lett kézbesítve, mert a küldő IP-cím biztonságosként lett megjelölve a kapcsolatszűrő házirendben.</span><span class="sxs-lookup"><span data-stu-id="d86d7-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="d86d7-104">A házirend áttekintéshez tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="d86d7-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="d86d7-105">Az [Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)Biztonsági & megfelelőségi központban, majd a Veszélyforrások elleni **védelem** házirend levélszemét  >    >  [elleni területén.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="d86d7-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="d86d7-106">Az Egyéni **lapon** válassza a Kapcsolatszűrő **házirend** lapjának Házirend **szerkesztése parancsát.**</span><span class="sxs-lookup"><span data-stu-id="d86d7-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="d86d7-107">Tekintse át az **IP Allow (Ip-cím engedélyezése)** listát.</span><span class="sxs-lookup"><span data-stu-id="d86d7-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="d86d7-108">Nézze **meg, hogy engedélyezve van-e** a Megbízható lista beállítás.</span><span class="sxs-lookup"><span data-stu-id="d86d7-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d86d7-109">A Microsoft előfizet a megbízható feladók külső forrásaira.</span><span class="sxs-lookup"><span data-stu-id="d86d7-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="d86d7-110">Ha **a Megbízható lista** engedélyezve van, a megbízható feladók nem lesznek tévesen levélszemétként megjelölve.</span><span class="sxs-lookup"><span data-stu-id="d86d7-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="d86d7-111">Ezt a beállítást javasoljuk, mert ezzel csökkenti a tévesen pozitív (tévesen levélszemétként osztályozott) üzenetek számát.</span><span class="sxs-lookup"><span data-stu-id="d86d7-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
