---
title: 1374 Két postaláda feloldása howto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1374"
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 95d85d7737ae0684b2a2c017134104bd377695f1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722520"
---
# <a name="a-user-has-two-mailboxes"></a><span data-ttu-id="cf013-102">Egy felhasználónak két postaládája van</span><span class="sxs-lookup"><span data-stu-id="cf013-102">A user has two mailboxes</span></span>

<span data-ttu-id="cf013-103">Az Azure Active Directory Connect (AAD Connect) vagy dirSync szolgáltatást használó hibrid környezetek véletlenül két postaládát okozhatnak a felhasználónak: egy helyszíni és egy a felhőben.</span><span class="sxs-lookup"><span data-stu-id="cf013-103">Hybrid environments that use Azure Active Directory Connect (AAD Connect) or DirSync might accidentally cause a user to have two mailboxes: one on-premises, and one in the cloud.</span></span> <span data-ttu-id="cf013-104">Mindkét helyen létrehozható ismétlődő postaláda.</span><span class="sxs-lookup"><span data-stu-id="cf013-104">A duplicate mailbox could be created in either place.</span></span>

<span data-ttu-id="cf013-105">A probléma megoldásához olvassa el [A postaláda helyreállítása az Exchange Online-ban és a helyszíni környezetben](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises)is.</span><span class="sxs-lookup"><span data-stu-id="cf013-105">To resolve this issue, see [How to recover when a mailbox exists in both Exchange Online and on-premises](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span></span> <span data-ttu-id="cf013-106">Ha többet szeretne megtudni arról, hogyan kerülheti el ezt a jövőben, olvassa el [a Saját felhasználó postaládája a helyszíni és az Exchange Online-ban című témakört. Segítünk!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809)</span><span class="sxs-lookup"><span data-stu-id="cf013-106">If you want to learn more about how to avoid this from happening in the future, see [My user has a mailbox both on-premises and in Exchange Online. Help!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span></span>
