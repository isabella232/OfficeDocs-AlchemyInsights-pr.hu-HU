---
title: A feltételes hozzáférésű figyelése
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538748"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="b14e9-102">Az Exchange felügyeleti feltételes hozzáférés</span><span class="sxs-lookup"><span data-stu-id="b14e9-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="b14e9-103">Célzott feltételes hozzáféréssel rendelkező felhasználók kapnak értesítést e-mailben, ha nem felel meg a szervezet hozzáférési követelmények.</span><span class="sxs-lookup"><span data-stu-id="b14e9-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b14e9-104">Úgy oldhatja meg, ajánlott egy vagy több a következő oldatokat:</span><span class="sxs-lookup"><span data-stu-id="b14e9-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="b14e9-105">Ha az eszköz feltételezhetőleg igényelt, tájékoztatja a felhasználót, hogy nyissa meg a vállalati portál app, és ellenőrizze, hogy a vállalati portál megjelenik.</span><span class="sxs-lookup"><span data-stu-id="b14e9-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b14e9-106">Ha nem, a felhasználó az eszközt kell igényelni.</span><span class="sxs-lookup"><span data-stu-id="b14e9-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="b14e9-107">Az Azure portálon Ugrás **Intune \> eszköz való**.</span><span class="sxs-lookup"><span data-stu-id="b14e9-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b14e9-108">Kattintson a **Monitor** **eszköz betartását**.</span><span class="sxs-lookup"><span data-stu-id="b14e9-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="b14e9-109">Ellenőrizze, hogy a felhasználó eszköz van megjelölve, kompatibilis az eszköz megfelelési jelentés megtekintése.</span><span class="sxs-lookup"><span data-stu-id="b14e9-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="b14e9-110">Az Azure portálon Ugrás **Intune \> eszköz való**.</span><span class="sxs-lookup"><span data-stu-id="b14e9-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b14e9-111">Kattintson a **Manage**, **házirendek**.</span><span class="sxs-lookup"><span data-stu-id="b14e9-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="b14e9-112">Megfelelés irányelveinek listája ellenőrizze, hogy a profil a felhasználó eszköz van rendelve.</span><span class="sxs-lookup"><span data-stu-id="b14e9-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b14e9-113">Ha nincs profil van rendelve, majd Intune nem tudják megfelelési Eszközállapot megerősítéséhez.</span><span class="sxs-lookup"><span data-stu-id="b14e9-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="b14e9-114">A felhasználó a feltételes hozzáférésű hozzárendelés szerkesztése.</span><span class="sxs-lookup"><span data-stu-id="b14e9-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="b14e9-115">Az Azure portálon Ugrás **Intune \> a feltételes hozzáférésű \> politika**</span><span class="sxs-lookup"><span data-stu-id="b14e9-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="b14e9-116">Jelölje ki a szabályzatot a listán</span><span class="sxs-lookup"><span data-stu-id="b14e9-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="b14e9-117">Kattintson a **felhasználók és csoportok**</span><span class="sxs-lookup"><span data-stu-id="b14e9-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="b14e9-118">Valaki, egy bizonyos házirend célozza meg, vegye fel őket a **belefoglalási** listába felvenni.</span><span class="sxs-lookup"><span data-stu-id="b14e9-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="b14e9-119">Annak érdekében, hogy egy személy a házirend nincs megadva, adja hozzá őket a **kizárása** listához.</span><span class="sxs-lookup"><span data-stu-id="b14e9-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="b14e9-120">További: [hogyan Monitor feltételes hozzáférést biztosító eszközök](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="b14e9-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

