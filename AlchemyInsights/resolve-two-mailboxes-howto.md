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
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 15723e0b9b98dbee5c8ad4d0417f86a03fa08c7e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "37026596"
---
# <a name="a-user-has-two-mailboxes"></a><span data-ttu-id="05b16-102">A felhasználónak két postaládájuk van</span><span class="sxs-lookup"><span data-stu-id="05b16-102">A user has two mailboxes</span></span>

<span data-ttu-id="05b16-103">Az Azure Active Directory Connect (AAD Connect) vagy a DirSync szolgáltatást használó hibrid környezetek miatt véletlenül a felhasználó két postaládát használhat: egy intézményi és egy a felhőben.</span><span class="sxs-lookup"><span data-stu-id="05b16-103">Hybrid environments that use Azure Active Directory Connect (AAD Connect) or DirSync might accidentally cause a user to have two mailboxes: one on-premises, and one in the cloud.</span></span> <span data-ttu-id="05b16-104">Duplikált postaláda hozható létre mindkét helyen.</span><span class="sxs-lookup"><span data-stu-id="05b16-104">A duplicate mailbox could be created in either place.</span></span>

<span data-ttu-id="05b16-105">A probléma megoldásához tekintse át, [Hogyan lehet helyreállítani egy postaládát az Exchange Online és a helyi létesítmények között](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span><span class="sxs-lookup"><span data-stu-id="05b16-105">To resolve this issue, see [How to recover when a mailbox exists in both Exchange Online and on-premises](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span></span> <span data-ttu-id="05b16-106">Ha többet szeretne megtudni arról, hogyan kerülheti el ezt a folyamatot a jövőben, tekintse meg a [felhasználók postaládáját a helyi és az Exchange Online webhelyen. Segíts!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span><span class="sxs-lookup"><span data-stu-id="05b16-106">If you want to learn more about how to avoid this from happening in the future, see [My user has a mailbox both on-premises and in Exchange Online. Help!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span></span>
