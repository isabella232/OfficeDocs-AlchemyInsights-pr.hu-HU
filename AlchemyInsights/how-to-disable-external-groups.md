---
title: Külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720770"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="d9cea-102">Külső csoportok letiltása</span><span class="sxs-lookup"><span data-stu-id="d9cea-102">How to disable External Groups</span></span>

<span data-ttu-id="d9cea-103">A Yammer külső üzenetküldése az Exchange transport rules (ETRs) szolgáltatást alkalmazza, amely proaktív vezérlők készlete a vállalati adatok megosztásának megakadályozására.</span><span class="sxs-lookup"><span data-stu-id="d9cea-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="d9cea-104">Annak érdekében, hogy a felhasználók ne hozzanak létre külső csoportokat, be kell állítania egy Exchange átviteli szabályt (ETR), majd be kell állítania a Yammert úgy, hogy az Exchange Transport szabályt használja a külső üzenetküldés letiltására.</span><span class="sxs-lookup"><span data-stu-id="d9cea-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="d9cea-105">Miután létrehozott egy szabályt az Exchange Online Felügyeleti központban, az alábbi lépésekkel állíthatja be az ETR-t a Yammerben való alkalmazáshoz:</span><span class="sxs-lookup"><span data-stu-id="d9cea-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="d9cea-106">Jelentkezzen be a Yammerbe ellenőrzött rendszergazdaként, és a **Yammer Felügyeleti központban**nyissa meg a C **tartalom- és biztonsági \> biztonsági beállítások at.**</span><span class="sxs-lookup"><span data-stu-id="d9cea-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="d9cea-107">A **Külső üzenetküldés**csoportban jelölje **be az Exchange Online Exchange átviteli szabályok (ETRs) érvényesítése a Yammerben jelölőnégyzetet.**</span><span class="sxs-lookup"><span data-stu-id="d9cea-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="d9cea-108">Válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="d9cea-108">Choose **Save**.</span></span>

<span data-ttu-id="d9cea-109">További információt a [Külső üzenetek letiltása Yammer-hálózatban](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="d9cea-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  