---
title: Bizonyos tartományoknak küldött Office 365-ös e-mailek automatikus titkosítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524876"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="a5649-102">Bizonyos tartományoknak küldött Office 365-ös e-mailek automatikus titkosítása</span><span class="sxs-lookup"><span data-stu-id="a5649-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="a5649-103">Az [Exchange Felügyeleti központban válassza](https://outlook.office365.com/ecp/)az **e-mail-forgalomra > szabályokat.**</span><span class="sxs-lookup"><span data-stu-id="a5649-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="a5649-104">Kattintson az **Új (+)** ikonra, majd az Office 365 Üzenettitkosítás és jogvédelem alkalmazása **az üzenetekre parancsra.**</span><span class="sxs-lookup"><span data-stu-id="a5649-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="a5649-105">A **Név** formában adja meg a szabály nevét, például a következő személynek küldött üzenetek *titkosítása contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="a5649-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="a5649-106">A **Szabály alkalmazása, ha** a tartomány **címzettje >** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a5649-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="a5649-107">Írja be a tartomány nevét, például **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="a5649-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="a5649-108">Kattintson a **Hozzáadás (+)** ikonra, majd az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="a5649-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="a5649-109">A Következő mező **mellett** kattintson az **Egyik kijelölése gombra.**</span><span class="sxs-lookup"><span data-stu-id="a5649-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="a5649-110">Az **RmS sablon legördülő** menüjében válassza a Titkosítás **lehetőséget,** majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="a5649-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="a5649-111">(Ha nem látja ezt a lehetőséget, az azt jelenti, hogy a csomagja nem tartalmaz automatikus titkosítást.</span><span class="sxs-lookup"><span data-stu-id="a5649-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="a5649-112">De hozzáadhatja!)</span><span class="sxs-lookup"><span data-stu-id="a5649-112">But you can add it!)</span></span>
9. <span data-ttu-id="a5649-113">Tetszőlegesen választhat (az ezen a ponton választható választható beállítások listájából, amelyek közül sok az egyszerűség alapértelmezett beállításával hagyható meg).</span><span class="sxs-lookup"><span data-stu-id="a5649-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="a5649-114">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="a5649-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a5649-115">Később mindig visszajöhet, és szerkesztheti ezt a szabályt.</span><span class="sxs-lookup"><span data-stu-id="a5649-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="a5649-116">További információ a titkosítási szabályok létrehozásáról: E-mail-forgalom szabályainak meghatározása az e-mailek titkosításához az [Office 365-ben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="a5649-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>