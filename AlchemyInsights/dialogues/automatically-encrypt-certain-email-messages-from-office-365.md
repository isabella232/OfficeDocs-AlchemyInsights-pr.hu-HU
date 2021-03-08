---
title: Bizonyos e-mailek automatikus titkosítása az Office 365-ben
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524912"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="6ff1b-102">Bizonyos e-mailek automatikus titkosítása az Office 365-ben</span><span class="sxs-lookup"><span data-stu-id="6ff1b-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="6ff1b-103">Az [Exchange Felügyeleti központban válassza](https://outlook.office365.com/ecp/)az **e-mail-forgalomra > szabályokat.**</span><span class="sxs-lookup"><span data-stu-id="6ff1b-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="6ff1b-104">Kattintson az **Új (+)** ikonra, majd az Office 365 Üzenettitkosítás és jogvédelem alkalmazása **az üzenetekre parancsra.**</span><span class="sxs-lookup"><span data-stu-id="6ff1b-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="6ff1b-105">A **Név** formában adja meg a szabály nevét, például az összes *üzenet titkosítása.*</span><span class="sxs-lookup"><span data-stu-id="6ff1b-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="6ff1b-106">A **Szabály alkalmazása, ha** a **[Mindegyik üzenetre]** lehetőséget választja.</span><span class="sxs-lookup"><span data-stu-id="6ff1b-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="6ff1b-107">A Következő mező **mellett** kattintson az **Egyik kijelölése gombra.**</span><span class="sxs-lookup"><span data-stu-id="6ff1b-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="6ff1b-108">Az **RmS sablon legördülő** menüjében válassza a Titkosítás **lehetőséget,** majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="6ff1b-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="6ff1b-109">(Ha nem látja ezt a lehetőséget, az azt jelenti, hogy a csomagja nem tartalmaz automatikus titkosítást.</span><span class="sxs-lookup"><span data-stu-id="6ff1b-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="6ff1b-110">De hozzáadhatja!)</span><span class="sxs-lookup"><span data-stu-id="6ff1b-110">But you can add it!)</span></span>
7. <span data-ttu-id="6ff1b-111">Jelölje be **a Szabályvizsgálat súlyossági** szinttel jelölőnégyzetet, majd válassza ki a kívánt szintet.</span><span class="sxs-lookup"><span data-stu-id="6ff1b-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="6ff1b-112">Ha vállalata szerződési kötelezettségekkel rendelkezik az összes e-mail titkosított küldésére, azt javasoljuk, hogy a szintet Magasra **kell omítani.**</span><span class="sxs-lookup"><span data-stu-id="6ff1b-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="6ff1b-113">A **Szabály típusának kiválasztása gombra** kattintva válassza a **Kényszerítés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6ff1b-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="6ff1b-114">Tetszőlegesen választhat (az ezen a ponton választható választható beállítások listájából, amelyek közül sok az egyszerűség alapértelmezett beállításával hagyható meg).</span><span class="sxs-lookup"><span data-stu-id="6ff1b-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="6ff1b-115">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="6ff1b-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6ff1b-116">Később mindig visszajöhet, és szerkesztheti ezt a szabályt.</span><span class="sxs-lookup"><span data-stu-id="6ff1b-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="6ff1b-117">További információ a titkosítási szabályok létrehozásáról: E-mail-forgalom szabályainak meghatározása az e-mailek titkosításához az [Office 365-ben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="6ff1b-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

