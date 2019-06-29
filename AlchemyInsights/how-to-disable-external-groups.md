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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384827"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="a2bb8-102">Külső csoportok letiltása</span><span class="sxs-lookup"><span data-stu-id="a2bb8-102">How to disable External Groups</span></span>

<span data-ttu-id="a2bb8-103">Yammer külső üzenetküldő Exchange átviteli szabályok – (ETR), a proaktív vezérlők vállalati adatok megosztását, elkerülésére vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="a2bb8-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="a2bb8-104">Annak érdekében, hogy korlátozza a felhasználók külső csoportok létrehozását, kell konfigurálása az Exchange átviteli szabály (ETR), és állítsa be az Exchange átviteli szabály segítségével blokkolja a külső üzenetküldő Yammer.</span><span class="sxs-lookup"><span data-stu-id="a2bb8-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="a2bb8-105">Exchange Online admin center szabály létrehozása után a következő lépésekkel állítsa be az ETR Yammer alkalmaz:</span><span class="sxs-lookup"><span data-stu-id="a2bb8-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="a2bb8-106">Bejelentkezés Yammer ellenőrzött admin, és **admin center Yammer**, ugorjon a C **tartalom és a biztonsági \> biztonsági beállításokat.**</span><span class="sxs-lookup"><span data-stu-id="a2bb8-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="a2bb8-107">A **Külső üzenetküldő**, válassza a **az Exchange Online Exchange közlekedési szabályok érvényesítése – (ETR) a Yammer.**</span><span class="sxs-lookup"><span data-stu-id="a2bb8-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="a2bb8-108">Válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="a2bb8-108">Choose **Save**.</span></span>

<span data-ttu-id="a2bb8-109">További tudnivalókért tanulmányozza a [külső üzenetküldő Exchange átviteli szabályok Yammer hálózati vezérlő](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="a2bb8-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  