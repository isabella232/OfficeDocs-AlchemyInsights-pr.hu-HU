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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694167"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="d7686-102">Kapcsolati házirend kijavítás</span><span class="sxs-lookup"><span data-stu-id="d7686-102">Fix connection policy</span></span>

<span data-ttu-id="d7686-103">Az e-mail biztonságosként lett megjelölve, és a felhasználó beérkezett üzenetek mappájába lett kézbesítve, mert a küldéshez szükséges IP-címet a Kapcsolatszűrő házirend biztonságosként jelölte meg.</span><span class="sxs-lookup"><span data-stu-id="d7686-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="d7686-104">A házirend áttekintéshez tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="d7686-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="d7686-105">Válassza az [Office 365 Biztonsági & megfelelőségi központot,](https://go.microsoft.com/fwlink/p/?linkid=2077143)majd a   >  Veszélyforrás-kezelési **házirend** levélszemét elleni  >  [védelem szolgáltatását.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="d7686-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="d7686-106">Az Egyéni **lapon** válassza a Kapcsolatszűrő **házirendet,** majd a Házirend **szerkesztése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d7686-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="d7686-107">Tekintse át az **IP Allow (Ip Engedélyezése)** listát.</span><span class="sxs-lookup"><span data-stu-id="d7686-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="d7686-108">Nézze **meg, hogy engedélyezve van-e** a megbízható lista.</span><span class="sxs-lookup"><span data-stu-id="d7686-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d7686-109">A Microsoft előfizet a megbízható feladók külső forrásaira.</span><span class="sxs-lookup"><span data-stu-id="d7686-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="d7686-110">Ha **a Megbízható feladók** lista engedélyezve van, a megbízható feladók nem lesznek tévesen levélszemétként megjelölve.</span><span class="sxs-lookup"><span data-stu-id="d7686-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="d7686-111">Azt javasoljuk, hogy ezt a beállítást válassza, mert ezzel csökkenti a kapott hamis pozitív üzenetek (levélszemétként osztályozott) számát.</span><span class="sxs-lookup"><span data-stu-id="d7686-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
