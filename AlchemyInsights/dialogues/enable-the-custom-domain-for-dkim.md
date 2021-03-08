---
title: A DKIM egyéni tartományának engedélyezése
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524128"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="64b79-102">A DKIM egyéni tartományának engedélyezése</span><span class="sxs-lookup"><span data-stu-id="64b79-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="64b79-103">Az egyéni tartományok CNAME rekordjainak létrehozása után engedélyeznie kell a tartományt.</span><span class="sxs-lookup"><span data-stu-id="64b79-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="64b79-104">A tartomány engedélyezéséhez végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="64b79-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="64b79-105">Nyissa meg az [Exchange Felügyeleti központot.](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="64b79-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="64b79-106">A bal oldali ablaktáblában válassza a **> dkim lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="64b79-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="64b79-107">Jelölje ki a tartományt, majd a tartományhoz az Üzenetek aláírása **DKIM-aláírással** csoportban kattintson az **Engedélyezés gombra.**</span><span class="sxs-lookup"><span data-stu-id="64b79-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="64b79-108">Ismételje meg ezt a lépést minden tartomány esetén.</span><span class="sxs-lookup"><span data-stu-id="64b79-108">Repeat this step for each domain.</span></span>

