---
title: Külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36739495"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="2ff4b-102">Külső csoportok letiltása</span><span class="sxs-lookup"><span data-stu-id="2ff4b-102">How to disable External Groups</span></span>

<span data-ttu-id="2ff4b-103">A yammer külső üzenetküldő szolgáltatás az Exchange átviteli szabályokat (ETRs), a vállalati adatok megosztásának megakadályozásához proaktív vezérlőket alkalmaz.</span><span class="sxs-lookup"><span data-stu-id="2ff4b-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="2ff4b-104">Ahhoz, hogy a felhasználók külső csoportokat is létrehozhassák, konfigurálnia kell az Exchange átviteli szabályt (ETR), majd konfigurálnia kell a Yammer programot az Exchange átviteli szabály használatára a külső üzenetek blokkolásához.</span><span class="sxs-lookup"><span data-stu-id="2ff4b-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="2ff4b-105">Miután létrehozott egy szabályt az Exchange Online admin központban, kövesse az alábbi lépéseket az ETR beállításához a Yammer esetében:</span><span class="sxs-lookup"><span data-stu-id="2ff4b-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="2ff4b-106">Jelentkezzen be Yammer-be ellenőrzött adminisztrátorként, és a **yammer Admin Center**, menjen a C **tartalom-és biztonsági \> beállítások.**</span><span class="sxs-lookup"><span data-stu-id="2ff4b-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="2ff4b-107">A **külső üzenetek**területen válassza **az Exchange Online Exchange-átviteli szabályok (Etrs) érvényesítése a yammer-ben.**</span><span class="sxs-lookup"><span data-stu-id="2ff4b-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="2ff4b-108">Válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="2ff4b-108">Choose **Save**.</span></span>

<span data-ttu-id="2ff4b-109">További információt a [külső üzenetkezelés letiltása Yammer hálózatban](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="2ff4b-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  