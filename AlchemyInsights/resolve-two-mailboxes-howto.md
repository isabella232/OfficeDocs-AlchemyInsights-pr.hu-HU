---
title: 1374 megoldása két postaláda howto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/2/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1374"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 1307e13bf76e0b2afc9038333533d708f5d12f7f
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992071"
---
# <a name="a-user-has-two-mailboxes"></a><span data-ttu-id="f0069-102">A felhasználónak két postaládájuk van</span><span class="sxs-lookup"><span data-stu-id="f0069-102">A user has two mailboxes</span></span>

<span data-ttu-id="f0069-103">Az Azure Active Directory Connect (AAD Connect) vagy a DirSync szolgáltatást használó hibrid környezetek miatt véletlenül a felhasználó két postaládát használhat: egy intézményi és egy a felhőben.</span><span class="sxs-lookup"><span data-stu-id="f0069-103">Hybrid environments that use Azure Active Directory Connect (AAD Connect) or DirSync might accidentally cause a user to have two mailboxes: one on-premises, and one in the cloud.</span></span> <span data-ttu-id="f0069-104">Duplikált postaláda hozható létre mindkét helyen.</span><span class="sxs-lookup"><span data-stu-id="f0069-104">A duplicate mailbox could be created in either place.</span></span>

<span data-ttu-id="f0069-105">A probléma megoldásához tekintse át, [Hogyan lehet helyreállítani egy postaládát az Exchange Online és a helyi létesítmények között](https://docs.microsoft.com/en-us/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span><span class="sxs-lookup"><span data-stu-id="f0069-105">To resolve this issue, see [How to recover when a mailbox exists in both Exchange Online and on-premises](https://docs.microsoft.com/en-us/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span></span> <span data-ttu-id="f0069-106">Ha többet szeretne megtudni arról, hogyan kerülhető el ez a jövőben, tekintse meg a [felhasználó postaládáját a helyi és az Exchange Online webhelyen. Segíts!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span><span class="sxs-lookup"><span data-stu-id="f0069-106">If you want to learn more about how to avoid this from happening in the future, please see [My user has a mailbox both on-premises and in Exchange Online. Help!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span></span>

