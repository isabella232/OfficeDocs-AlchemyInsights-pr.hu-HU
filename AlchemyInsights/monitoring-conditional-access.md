---
title: Feltételes hozzáférés figyelése
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702905"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="7ca6f-102">Feltételes hozzáférés figyelése az Exchange-ben</span><span class="sxs-lookup"><span data-stu-id="7ca6f-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="7ca6f-103">A feltételes hozzáféréssel célzott felhasználók értesítést kapnak e-mailben, ha nem felelnek meg a szervezet hozzáférési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="7ca6f-104">A probléma megoldásához az alábbi megoldások közül legalább egyet ajánlunk:</span><span class="sxs-lookup"><span data-stu-id="7ca6f-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="7ca6f-105">Ha az eszköz feltételezetten regisztrált, értesítse a felhasználót, hogy nyissa meg a vállalati portál alkalmazást, és ellenőrizze, hogy megjelenik-e a vállalati portálon.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="7ca6f-106">Ha nem, akkor a felhasználónak regisztrálnia kell az eszközt.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="7ca6f-107">Az Azure portálon nyissa meg a **Intune \> eszköz megfelelősége**című részt.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="7ca6f-108">A **monitor** csoportban kattintson az **eszköz megfelelősége**elemre.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="7ca6f-109">Tekintse meg az eszköz megfelelőségi jelentését annak ellenőrzéséhez, hogy a felhasználó eszközének megfelelően van-e megjelölve.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="7ca6f-110">Az Azure portálon nyissa meg a **Intune \> eszköz megfelelősége**című részt.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="7ca6f-111">A **kezelés**csoportban kattintson a **házirendek**elemre.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="7ca6f-112">Ellenőrizze, hogy a megfelelőségi házirendek listája tartalmazza-e a felhasználói eszközhöz tartozó profilt.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="7ca6f-113">Ha nincs kiosztva profil, akkor a Intune nem fogja tudni ellenőrizni az eszköz megfelelőségi állapotát.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="7ca6f-114">Módosítsa a felhasználó feltételes hozzáférés-hozzárendelését.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="7ca6f-115">Az Azure portálon nyissa meg az **Intune \> feltételes hozzáférési \> házirendeket**</span><span class="sxs-lookup"><span data-stu-id="7ca6f-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="7ca6f-116">Házirend kijelölése a listából</span><span class="sxs-lookup"><span data-stu-id="7ca6f-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="7ca6f-117">Kattintson **a felhasználók és csoportok** elemre.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="7ca6f-118">Ha egy bizonyos házirendet valakinek szeretne célozni, vegye fel őket a **belefoglalási** listára.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="7ca6f-119">Ha meg szeretne győződni arról, hogy egy személy nincs kihagyva a házirendből, vegye fel őket a **kizárási** listára.</span><span class="sxs-lookup"><span data-stu-id="7ca6f-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="7ca6f-120">További információ: [feltételes hozzáférésű eszközök figyelése](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="7ca6f-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

