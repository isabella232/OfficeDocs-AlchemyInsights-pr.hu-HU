---
title: Feltételes hozzáférés figyelése
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713720"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="6a7d1-102">Az Exchange feltételes hozzáférésének figyelése</span><span class="sxs-lookup"><span data-stu-id="6a7d1-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="6a7d1-103">A feltételes hozzáféréssel rendelkező felhasználók értesítést kapnak e-mailben, ha nem felelnek meg a szervezet hozzáférési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6a7d1-104">A megoldáshoz az alábbi megoldások közül választhat:</span><span class="sxs-lookup"><span data-stu-id="6a7d1-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="6a7d1-105">Ha az eszköz vélelmezni kell, hogy regisztrált, javasoljuk a felhasználónak, hogy menjen a Céges portál alkalmazást, és ellenőrizze, hogy megjelenik-e a céges portálon.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6a7d1-106">Ha nem, a felhasználónak regisztrálnia kell az eszközt.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="6a7d1-107">Az Azure Portalon nyissa meg az **Intune-eszköz \> megfelelősége.**</span><span class="sxs-lookup"><span data-stu-id="6a7d1-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6a7d1-108">A **Figyelő** csoportban kattintson **az Eszközmegfelelőség**elemre.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="6a7d1-109">Tekintse meg az eszköz megfelelőségi jelentését, és ellenőrizze, hogy a felhasználó eszköze megfelelőként van-e megjelölve.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="6a7d1-110">Az Azure Portalon nyissa meg az **Intune-eszköz \> megfelelősége.**</span><span class="sxs-lookup"><span data-stu-id="6a7d1-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6a7d1-111">A **Kezelés csoportban**kattintson a **Házirendek**gombra.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="6a7d1-112">A megfelelőségi szabályzatok listájában ellenőrizze, hogy egy profil hozzá van-e rendelve a felhasználó eszközéhez.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6a7d1-113">Ha nincs hozzárendelve profil, akkor az Intune nem fogja tudni megerősíteni az eszköz megfelelőségi állapotát.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="6a7d1-114">A felhasználó feltételes hozzáférési hozzárendelésének szerkesztése.</span><span class="sxs-lookup"><span data-stu-id="6a7d1-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="6a7d1-115">Az Azure Portalon nyissa meg az **Intune \> feltételes hozzáférési \> szabályzatait**</span><span class="sxs-lookup"><span data-stu-id="6a7d1-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="6a7d1-116">Házirend kiválasztása a listából</span><span class="sxs-lookup"><span data-stu-id="6a7d1-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="6a7d1-117">Kattintson **a Felhasználók és csoportok elemre.**</span><span class="sxs-lookup"><span data-stu-id="6a7d1-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="6a7d1-118">Ha egy bizonyos házirendet meg szeretne célozni valakire, vegye fel a **Belefoglalás listára.**</span><span class="sxs-lookup"><span data-stu-id="6a7d1-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="6a7d1-119">Annak érdekében, hogy egy személy kikerüljön a házirendből, vegye fel őket a **Kizárás listára.**</span><span class="sxs-lookup"><span data-stu-id="6a7d1-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="6a7d1-120">További információ: [A feltételes hozzáférésű eszközök figyelése](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="6a7d1-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

