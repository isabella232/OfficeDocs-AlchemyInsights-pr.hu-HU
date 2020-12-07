---
title: Mi a teendő, ha az Azure-funkciók nem működnek megfelelően a Microsoft Edge-ben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583460"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="47c17-102">Mi a teendő, ha az Azure-funkciók nem működnek megfelelően a Microsoft Edge-ben</span><span class="sxs-lookup"><span data-stu-id="47c17-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="47c17-103">A Microsoft Edge [ismert problémákkal](https://go.microsoft.com/fwlink/?linkid=2140608) bír, amelyek a biztonsági zónákhoz kapcsolódnak, és befolyásolhatják, hogy az Azure-felhasználók hogyan jelentkezzenek be a Windows felügyeleti központba.</span><span class="sxs-lookup"><span data-stu-id="47c17-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="47c17-104">Ha problémát tapasztal az Azure-funkciók Microsoft Edge-ben való használatakor, próbálkozzon az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="47c17-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="47c17-105">A **Start** menüben keresse meg az **Internetbeállítások lehetőséget** , és jelölje ki.</span><span class="sxs-lookup"><span data-stu-id="47c17-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="47c17-106">Az **Internet tulajdonságai** párbeszédpanelen lépjen a **Biztonság** lapra.</span><span class="sxs-lookup"><span data-stu-id="47c17-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="47c17-107">Jelölje ki a **megbízható helyek** zónát, és válassza a **webhelyek** gombot.</span><span class="sxs-lookup"><span data-stu-id="47c17-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="47c17-108">A **megbízható helyek** párbeszédpanelen adja meg az átjáró URL-címét, és [https://login.microsoftonline.com](https://login.microsoftonline.com) válassza a [https://login.live.com](https://login.live.com) **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="47c17-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="47c17-109">Az **Internet tulajdonságai** párbeszédpanelen lépjen az **Adatvédelem** lapra.</span><span class="sxs-lookup"><span data-stu-id="47c17-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="47c17-110">Az **előugró ablakok blokkolása** csoportban válassza a **Beállítások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="47c17-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="47c17-111">A megnyíló párbeszédpanelen adja meg az átjáró URL-címét, és [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="47c17-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
