---
title: Replikakészlet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714248"
---
# <a name="replica-set"></a><span data-ttu-id="ec0c6-102">Replikakészlet</span><span class="sxs-lookup"><span data-stu-id="ec0c6-102">Replica set</span></span>

<span data-ttu-id="ec0c6-103">Az AADDS-t felügyelt tartománynak is nevezik.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="ec0c6-104">Valójában két tartományvezérlőt futtat és tart fenn a háttérkiszolgáló.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="ec0c6-105">A két DCs egy fő tartományvezérlőt és egy replikációs tartományvezérlőt tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="ec0c6-106">Az AADDS (felügyelt tartomány) biztonsági másolatai az Azure platform által kezelt automatizált folyamatok.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="ec0c6-107">Ha probléma ad problémát a felügyelt tartománnyal, az Azure ügyfélszolgálata segítséget nyújthat a biztonsági másolatból való visszaállításban.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="ec0c6-108">Minden egyes replikakészletet egy virtuális hálózaton hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="ec0c6-109">Minden virtuális hálózatnak társviszonyban kell lennie minden más olyan virtuális hálózattal, amely a felügyelt tartomány replikakészletét kezeli.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="ec0c6-110">Ez a konfiguráció hálóhálózati topológiát hoz létre, amely támogatja a címtár-replikációt.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="ec0c6-111">A virtuális hálózatok több replikakészletet is támogatnak, feltéve, hogy minden egyes replikakészlet egy másik virtuális alhálózatban található.</span><span class="sxs-lookup"><span data-stu-id="ec0c6-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="ec0c6-112">A Replikakészlettel kapcsolatos további információkért lásd [a "Concepts Replikakészletek" halmazt.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="ec0c6-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
