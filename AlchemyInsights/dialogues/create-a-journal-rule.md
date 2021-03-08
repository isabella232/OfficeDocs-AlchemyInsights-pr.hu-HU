---
title: Naplószabály létrehozása
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: b0b95f8b6460418d92314dede2ca8bc1326b033e
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524807"
---
# <a name="create-a-journal-rule"></a><span data-ttu-id="0e2bf-102">Naplószabály létrehozása</span><span class="sxs-lookup"><span data-stu-id="0e2bf-102">Create a journal rule</span></span>

<span data-ttu-id="0e2bf-103">Ezt a következőképpen teheti meg:</span><span class="sxs-lookup"><span data-stu-id="0e2bf-103">Here's how:</span></span>

1. <span data-ttu-id="0e2bf-104">Az [Exchange Felügyeleti központban](https://go.microsoft.com/fwlink/p/?linkid=2059104)válassza a **megfelelőségkezelési** naplószabályokat, majd válassza a Hozzáadás  >   **(+)** ikont.</span><span class="sxs-lookup"><span data-stu-id="0e2bf-104">In the [Exchange admin center](https://go.microsoft.com/fwlink/p/?linkid=2059104), go to **compliance management** > **journal rules**, and then select the **Add (+)** icon.</span></span>
2. <span data-ttu-id="0e2bf-105">Az **új naplószabályban** adjon nevet a naplószabálynak, majd versenyezzen az alábbi mezőkkel:</span><span class="sxs-lookup"><span data-stu-id="0e2bf-105">In **new journal rule**, provide a name for the journal rule and then compete the following fields:</span></span>  
    - <span data-ttu-id="0e2bf-106">**Naplójelentések küldése a következő címre:** Adja meg annak a naplópostafióknak a címét, amely az összes naplójelentést megkapja.</span><span class="sxs-lookup"><span data-stu-id="0e2bf-106">**Send journal reports to**: Enter the address of the journaling mailbox that will receive all the journal reports.</span></span>  
    - <span data-ttu-id="0e2bf-107">**Ha az üzenet címzettje vagy címzettje a** következő: Adja meg a címzettet, akire a szabály vonatkozni fog.</span><span class="sxs-lookup"><span data-stu-id="0e2bf-107">**If the message is sent to or received from**: Specify the recipient that the rule will target.</span></span> <span data-ttu-id="0e2bf-108">Kijelölhet egy adott címzettet, vagy alkalmazhatja a szabályt az összes üzenetre.</span><span class="sxs-lookup"><span data-stu-id="0e2bf-108">You can either select a specific recipient or apply the rule to all messages.</span></span>  
    - <span data-ttu-id="0e2bf-109">**A következő üzenetek naplózása:** Adja meg a naplószabály hatókörét.</span><span class="sxs-lookup"><span data-stu-id="0e2bf-109">**Journal the following messages**: Specify the scope of the journal rule.</span></span> <span data-ttu-id="0e2bf-110">Csak a belső üzeneteket, csak a külső üzeneteket vagy az összes üzenetet naplólhatja, függetlenül a forrástól vagy a céltól.</span><span class="sxs-lookup"><span data-stu-id="0e2bf-110">You can journal only the internal messages, only the external messages, or all messages regardless of origin or destination.</span></span>
3. <span data-ttu-id="0e2bf-111">Válassza **a Mentés gombot** a naplószabály létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="0e2bf-111">Select **Save** to create the journal rule.</span></span>
