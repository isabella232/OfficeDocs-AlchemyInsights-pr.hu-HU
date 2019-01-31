---
title: Külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 09d8b134a4e99912301aa92c2e989fec9dd30a7b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656389"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="f9d1e-102">Külső csoportok letiltása</span><span class="sxs-lookup"><span data-stu-id="f9d1e-102">How to disable External Groups</span></span>

<span data-ttu-id="f9d1e-p101">Yammer külső üzenetküldő Exchange átviteli szabályok – (ETR), a proaktív vezérlők vállalati adatok megosztását, elkerülésére vonatkozik. Annak érdekében, hogy korlátozza a felhasználók külső csoportok létrehozását, kell konfigurálása az Exchange átviteli szabály (ETR), és állítsa be az Exchange átviteli szabály segítségével blokkolja a külső üzenetküldő Yammer.</span><span class="sxs-lookup"><span data-stu-id="f9d1e-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="f9d1e-105">Exchange Online admin center szabály létrehozása után a következő lépésekkel állítsa be az ETR Yammer alkalmaz:</span><span class="sxs-lookup"><span data-stu-id="f9d1e-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="f9d1e-106">Bejelentkezés Yammer ellenőrzött admin, és **admin center Yammer**, ugorjon a C **ontent és biztonsági \> biztonsági beállításokat.**</span><span class="sxs-lookup"><span data-stu-id="f9d1e-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="f9d1e-107">A **Külső üzenetküldő**, válassza a **az Exchange Online Exchange közlekedési szabályok érvényesítése – (ETR) a Yammer.**</span><span class="sxs-lookup"><span data-stu-id="f9d1e-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="f9d1e-108">Válassza a **Save** (Mentés) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f9d1e-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="f9d1e-109">További tudnivalókért tanulmányozza a [külső üzenetküldő Exchange átviteli szabályok Yammer hálózati vezérlő](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="f9d1e-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

