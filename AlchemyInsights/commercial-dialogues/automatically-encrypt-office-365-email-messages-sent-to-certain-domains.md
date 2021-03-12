---
title: Bizonyos tartományokra küldött Office 365-ös e-mailek automatikus titkosítása
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746050"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="68b83-102">Bizonyos tartományokra küldött Office 365-ös e-mailek automatikus titkosítása</span><span class="sxs-lookup"><span data-stu-id="68b83-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="68b83-103">Az [Exchange Felügyeleti központban válassza](https://outlook.office365.com/ecp/)az **e-mail-forgalom és > lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="68b83-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="68b83-104">Kattintson az **Új (+)** ikonra, majd az **Office 365** Üzenettitkosítás és jogvédelem alkalmazása az üzenetekre elemre.</span><span class="sxs-lookup"><span data-stu-id="68b83-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="68b83-105">A **Név** formában adja meg a szabály nevét, például a következőnek küldött üzenetek *titkosítása contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="68b83-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="68b83-106">A **Szabály alkalmazása, ha területen** válassza A címzett > **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="68b83-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="68b83-107">Írja be a tartomány nevét, például **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="68b83-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="68b83-108">Kattintson **a Hozzáadás (+)** ikonra, majd az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="68b83-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="68b83-109">A következő **lépés mező mellett** kattintson a Válasszon **gombra.**</span><span class="sxs-lookup"><span data-stu-id="68b83-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="68b83-110">Az **RMS sablon legördülő** menüjében válassza a **Titkosítás** elemet, majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="68b83-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="68b83-111">(Ha nem látja ezt a beállítást, az azt jelenti, hogy a csomagja nem tartalmaz automatikus titkosítást.</span><span class="sxs-lookup"><span data-stu-id="68b83-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="68b83-112">De ön is hozzáadhatja!)</span><span class="sxs-lookup"><span data-stu-id="68b83-112">But you can add it!)</span></span>
9. <span data-ttu-id="68b83-113">Válasszon a választható beállítások közül (az ezen a ponton választható beállítások listájából, amelyek közül sok az egyszerűség alapértelmezett beállításával hagyható meg).</span><span class="sxs-lookup"><span data-stu-id="68b83-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="68b83-114">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="68b83-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="68b83-115">A szabályt később is mindig módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="68b83-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="68b83-116">A titkosítási szabályok létrehozásáról további információt az E-mail-forgalom szabályainak megadása az [Office 365-ben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) az e-mailek titkosításához</span><span class="sxs-lookup"><span data-stu-id="68b83-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>