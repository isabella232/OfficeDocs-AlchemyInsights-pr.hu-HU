---
title: Bizonyos Office 365-ös e-mailek automatikus titkosítása
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524900"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="77940-102">Bizonyos Office 365-ös e-mailek automatikus titkosítása</span><span class="sxs-lookup"><span data-stu-id="77940-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="77940-103">Automatikusan titkosíthatja a felhasználók által bizonyos külső személyeknek vagy szervezeteknek küldött üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="77940-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="77940-104">Ehhez végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="77940-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="77940-105">Az [Exchange Felügyeleti központban válassza](https://outlook.office365.com/ecp/)az **e-mail-forgalomra > szabályokat.**</span><span class="sxs-lookup"><span data-stu-id="77940-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="77940-106">Kattintson az **Új (+)** ikonra, majd az Office 365 Üzenettitkosítás és jogvédelem alkalmazása **az üzenetekre parancsra.**</span><span class="sxs-lookup"><span data-stu-id="77940-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="77940-107">A **Név** formában adja meg a szabály nevét, például a következőnek küldött üzenetek *titkosítása DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="77940-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="77940-108">Ha **a Szabály alkalmazása** lehetőséget választja, válassza az > **címzettet.**</span><span class="sxs-lookup"><span data-stu-id="77940-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="77940-109">A **Tagok kiválasztása** ablakban jelölje ki annak a személynek a nevét, akire alkalmazni szeretné a titkosítási szabályt, majd kattintson a **Hozzáadás gombra.**</span><span class="sxs-lookup"><span data-stu-id="77940-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="77940-110">Ha végzett a felhasználók felvételének, kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="77940-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="77940-111">A Következő mező **mellett** kattintson az **Egyik kijelölése gombra.**</span><span class="sxs-lookup"><span data-stu-id="77940-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="77940-112">Az **RmS sablon legördülő** menüjében válassza a Titkosítás **lehetőséget,** majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="77940-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="77940-113">(Ha nem látja ezt a lehetőséget, az azt jelenti, hogy a csomagja nem tartalmaz automatikus titkosítást.</span><span class="sxs-lookup"><span data-stu-id="77940-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="77940-114">De hozzáadhatja!)</span><span class="sxs-lookup"><span data-stu-id="77940-114">But you can add it!)</span></span>
9. <span data-ttu-id="77940-115">Tetszőlegesen választhat (az ezen a ponton választható választható beállítások listájából, amelyek közül sok az egyszerűség alapértelmezett beállításával hagyható meg).</span><span class="sxs-lookup"><span data-stu-id="77940-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="77940-116">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="77940-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="77940-117">Később mindig visszajöhet, és szerkesztheti ezt a szabályt.</span><span class="sxs-lookup"><span data-stu-id="77940-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="77940-118">A titkosítási szabályok létrehozásáról további információt az E-mail-forgalom szabályainak meghatározása az [e-mailek Office 365-ben való titkosításához.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="77940-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

