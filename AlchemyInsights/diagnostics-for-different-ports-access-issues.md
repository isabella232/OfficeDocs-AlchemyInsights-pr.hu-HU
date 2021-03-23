---
title: A különböző portokhoz való hozzáféréssel kapcsolatos problémák diagnosztika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035782"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="e759e-102">A különböző portokhoz való hozzáféréssel kapcsolatos problémák diagnosztika</span><span class="sxs-lookup"><span data-stu-id="e759e-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="e759e-103">A különböző portelérési problémák megoldásához végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="e759e-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="e759e-104">A virtuális gép (VM) leállítása/deallocate a portálról, indítsa újra a VM-et, és tesztelje újra.</span><span class="sxs-lookup"><span data-stu-id="e759e-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="e759e-105">A VM hálózati beállításait ellenőrizve állapítsa meg, hogy vannak-e hálózati biztonsági csoportok, amelyek letiltják a forgalmat.</span><span class="sxs-lookup"><span data-stu-id="e759e-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="e759e-106">A Network [Watcher IP-forgalom](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) ellenőrző eszközével is ellenőrizheti, hogy vannak-e olyan NSG-k, amelyek letiltják a forgalmat, a User-Defined Útvonalak (UDRs) a forgalmat a helyszíni környezetbe (0.0.0.0/0/0) vagy egy hálózati készülékhez irányítják vissza.</span><span class="sxs-lookup"><span data-stu-id="e759e-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="e759e-107">Ha a fenti lépések után is problémákat tapasztal, kérjük, adja meg a VM nevét és azt a TCP-portot, amelyről levelet próbál küldeni további probléma esetén.</span><span class="sxs-lookup"><span data-stu-id="e759e-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="e759e-108">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="e759e-108">**Recommended Documents**</span></span>

[<span data-ttu-id="e759e-109">Korlátozások és javaslatok a 25-ös porton keresztüli kimenő e-mailek küldésére</span><span class="sxs-lookup"><span data-stu-id="e759e-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)