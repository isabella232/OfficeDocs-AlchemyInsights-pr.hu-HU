---
title: Bérlői házirend kijavítása (művelet felülbírálása)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694062"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="7bca1-102">Bérlői házirend kijavítása (művelet felülbírálása)</span><span class="sxs-lookup"><span data-stu-id="7bca1-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="7bca1-103">Ezt az üzenetet egy levélszemét-szűrési házirend érintette a bérlői webhelyen.</span><span class="sxs-lookup"><span data-stu-id="7bca1-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="7bca1-104">A házirend áttekintéshez tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="7bca1-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="7bca1-105">Válassza az [Office 365 Biztonsági & megfelelőségi központot,](https://go.microsoft.com/fwlink/p/?linkid=2077143)majd a   >  Veszélyforrás-kezelési **házirend** levélszemét elleni  >  [védelem szolgáltatását.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="7bca1-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="7bca1-106">Ellenőrizze, hogy  a házirendforrás a következőt **jelzi-e: Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="7bca1-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="7bca1-107">Ha igen, az Egyéni **lapon** ellenőrizze az üzenetre vonatkozó házirend beállításait.</span><span class="sxs-lookup"><span data-stu-id="7bca1-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="7bca1-108">Lehetséges, hogy az  Exchange Online Védelmi szolgáltatás minden ügyfele számára érvényes szokásos beállítások hatással vannak az üzenetre.</span><span class="sxs-lookup"><span data-stu-id="7bca1-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="7bca1-109">A levélszemétszűrő házirendek konfigurálásával kapcsolatos további információkért [lásd: A levélszemétszűrő házirendek konfigurálása.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="7bca1-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
