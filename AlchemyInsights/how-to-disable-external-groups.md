---
title: A külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704130"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="0beef-102">A külső csoportok letiltása</span><span class="sxs-lookup"><span data-stu-id="0beef-102">How to disable External Groups</span></span>

<span data-ttu-id="0beef-103">Külső Yammer: az Exchange átviteli szabályait (ETR), a proaktív vezérlők halmazát, amelyekkel megakadályozhatja, hogy a vállalati adatok meg legyenek osztva.</span><span class="sxs-lookup"><span data-stu-id="0beef-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="0beef-104">Ha korlátozni szeretné, hogy a felhasználók külső csoportokat hozzanak létre, be kell állítania egy Exchange átviteli szabályt (ETR), majd konfigurálnia kell a Yammer, hogy az Exchange átviteli szabály segítségével tiltsa le a külső üzenetküldést.</span><span class="sxs-lookup"><span data-stu-id="0beef-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="0beef-105">Miután létrehozott egy szabályt az Exchange Online felügyeleti központban, az alábbi lépésekkel állíthatja be az ETR-t a Yammer alkalmazásban:</span><span class="sxs-lookup"><span data-stu-id="0beef-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="0beef-106">Jelentkezzen be a Yammer igazolt rendszergazdaként, és a **Yammer felügyeleti központban**lépjen a C **tartalom és biztonsági beállítások lapra \> .**</span><span class="sxs-lookup"><span data-stu-id="0beef-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="0beef-107">A **külső üzenetkezelés**csoportban jelölje be **az Exchange Online Exchange-átviteli szabályok (ETR) érvényesítése az Yammer-on** című témakört.</span><span class="sxs-lookup"><span data-stu-id="0beef-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="0beef-108">Válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="0beef-108">Choose **Save**.</span></span>

<span data-ttu-id="0beef-109">További információt a [külső üzenetküldés letiltása Yammer-hálózatban](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="0beef-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  