---
title: az 717 lehetővé teszi, hogy a felhasználók terjesztési listaként küldjenek e-maileket
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "717"
- "3"
ms.assetid: d9e5f5be-b653-44a9-bce8-9ca11396d39e
ms.openlocfilehash: 71f251139160ef41acac13fd08af80515581ea10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47718119"
---
# <a name="allow-users-to-send-email-as-a-distribution-group"></a><span data-ttu-id="913fd-102">E-mailek terjesztési csoportként való küldésének engedélyezése a felhasználóknak</span><span class="sxs-lookup"><span data-stu-id="913fd-102">Allow users to send email as a distribution group</span></span>

<span data-ttu-id="913fd-103">Ha engedélyezni szeretné, hogy a felhasználók olyan üzeneteket küldhessenek, amelyek egy meglévő terjesztési csoportból származnak, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="913fd-103">To allow users to send messages that appear to come from an existing distribution group, follow these steps:</span></span>

1. <span data-ttu-id="913fd-104">Az [Exchange admin centerban](https://outlook.office365.com/ecp/)lépjen a **címzettek** \> **csoportokra**.</span><span class="sxs-lookup"><span data-stu-id="913fd-104">In the [Exchange admin center](https://outlook.office365.com/ecp/), go to **Recipients** \> **Groups**.</span></span>

2. <span data-ttu-id="913fd-105">Jelölje ki azt a terjesztési csoportot, amelyet módosítani szeretne, majd kattintson a **Szerkesztés**elemre.</span><span class="sxs-lookup"><span data-stu-id="913fd-105">Select the distribution group you want to modify, and then click **Edit**.</span></span>

3. <span data-ttu-id="913fd-106">A csoport tulajdonságai között lépjen a **csoport delegálása** lapra, ahol megadhatja azokat a felhasználókat, akik a terjesztési csoport nevében küldhetnek vagy küldhetnek.</span><span class="sxs-lookup"><span data-stu-id="913fd-106">In the properties of the group, go to the **Group delegation** tab to specify the users who can send as or send on behalf of the distribution group.</span></span>

<span data-ttu-id="913fd-107">További információt az [e-mail-beállítások](https://technet.microsoft.com/library/bb124513.aspx#groupdelegation)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="913fd-107">For more information, see [Email options](https://technet.microsoft.com/library/bb124513.aspx#groupdelegation).</span></span>
