---
title: E-mailek automatikus áthelyezése az archív postaládába
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525095"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="18c44-102">E-mailek automatikus áthelyezése az archív postaládába</span><span class="sxs-lookup"><span data-stu-id="18c44-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="18c44-103">Így állíthat be olyan házirendet, amely automatikusan áthelyezi a felhasználók régi e-mailjeit az archív postaládába:</span><span class="sxs-lookup"><span data-stu-id="18c44-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="18c44-104">Ha ellenőrizni &, hogy engedélyezve van-e egy archív postaláda a felhasználó számára, menjen a Biztonsági [**&-**](https://go.microsoft.com/fwlink/p/?linkid=2077143)és megfelelőségi adatirányítási  >    >   archívumba.</span><span class="sxs-lookup"><span data-stu-id="18c44-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="18c44-105">Ha nem, a figyelmeztetésben kattintson az **Engedélyezés,** majd az **Igen** gombra.</span><span class="sxs-lookup"><span data-stu-id="18c44-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="18c44-106">Az [**Adatmegőrzési címkékkel > Exchange Felügyeleti központ > felügyeleti központot.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="18c44-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="18c44-107">Válassza a + ikont, majd válassza az **automatikus alkalmazás a teljes postaládára.**</span><span class="sxs-lookup"><span data-stu-id="18c44-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="18c44-108">Nevezze el az adatmegőrzési címkét, és válassza az **Áthelyezés az archívumba lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="18c44-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="18c44-109">Az adatmegőrzési időszakhoz adja meg a kívánt időt, például 90 napot.</span><span class="sxs-lookup"><span data-stu-id="18c44-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="18c44-110">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="18c44-110">Click **Save**.</span></span>
5. <span data-ttu-id="18c44-111">Most hozzon létre egy adatmegőrzési házirendet: válassza az **adatmegőrzési** házirendeket, majd az ikont választva vegyen fel egy új házirendet.</span><span class="sxs-lookup"><span data-stu-id="18c44-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="18c44-112">Adjon nevet az adatmegőrzési házirendnek, majd kattintással és görgetéssel keresse meg és vegye fel az éppen létrehozott adatmegőrzési címkét.</span><span class="sxs-lookup"><span data-stu-id="18c44-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="18c44-113">Kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="18c44-113">Click **Save**.</span></span>
7. <span data-ttu-id="18c44-114">Végül alkalmazza az adatmegőrzési házirendet a felhasználó postaládájában: az Exchange Felügyeleti központban maradva, a címzettek  >  **postaládáihoz.**</span><span class="sxs-lookup"><span data-stu-id="18c44-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="18c44-115">Jelölje ki az összes felhasználót, akire alkalmazni szeretné a házirendet, majd válassza a **Szerkesztés** (ceruza) ikont.</span><span class="sxs-lookup"><span data-stu-id="18c44-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="18c44-116">A párbeszédpanelen kattintson a **postaláda-szolgáltatások elemre.**</span><span class="sxs-lookup"><span data-stu-id="18c44-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="18c44-117">Az **Adatmegőrzési házirend** alatt alkalmazza a mentés > **házirendet.**</span><span class="sxs-lookup"><span data-stu-id="18c44-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="18c44-118">A házirend minden felhasználóra való alkalmazásával kapcsolatos utasításokat az Adatmegőrzési házirend alkalmazása [postaládákra.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="18c44-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
