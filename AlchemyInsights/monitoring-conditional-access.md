---
title: A feltételes hozzáférésű figyelése
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473051"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="15d0b-102">A feltételes hozzáférésű figyelése</span><span class="sxs-lookup"><span data-stu-id="15d0b-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="15d0b-p101">Célzott feltételes hozzáféréssel rendelkező felhasználók kapnak értesítést e-mailben, ha nem felel meg a szervezet hozzáférési követelmények. Úgy oldhatja meg, ajánlott egy vagy több a következő oldatokat:</span><span class="sxs-lookup"><span data-stu-id="15d0b-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="15d0b-p102">Ha az eszköz feltételezhetőleg igényelt, tájékoztatja a felhasználót, hogy nyissa meg a vállalati portál app, és ellenőrizze, hogy a vállalati portál megjelenik. Ha nem, a felhasználó az eszközt kell igényelni.</span><span class="sxs-lookup"><span data-stu-id="15d0b-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="15d0b-p103">Az Azure portálon Ugrás **Intune \> eszköz való**. Kattintson a **Monitor** **eszköz betartását**. Ellenőrizze, hogy a felhasználó eszköz van megjelölve, kompatibilis az eszköz megfelelési jelentés megtekintése.</span><span class="sxs-lookup"><span data-stu-id="15d0b-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="15d0b-p104">Az Azure portálon Ugrás **Intune \> eszköz való**. Kattintson a **Manage**, **házirendek**. Megfelelés irányelveinek listája ellenőrizze, hogy a profil a felhasználó eszköz van rendelve. Ha nincs profil van rendelve, majd Intune nem tudják megfelelési Eszközállapot megerősítéséhez.</span><span class="sxs-lookup"><span data-stu-id="15d0b-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="15d0b-114">A felhasználó a feltételes hozzáférésű hozzárendelés szerkesztése.</span><span class="sxs-lookup"><span data-stu-id="15d0b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="15d0b-115">Az Azure portálon Ugrás **Intune \> a feltételes hozzáférésű \> politika**</span><span class="sxs-lookup"><span data-stu-id="15d0b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="15d0b-116">Jelölje ki a szabályzatot a listán</span><span class="sxs-lookup"><span data-stu-id="15d0b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="15d0b-117">Kattintson a **felhasználók és csoportok**</span><span class="sxs-lookup"><span data-stu-id="15d0b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="15d0b-p105">Valaki, egy bizonyos házirend célozza meg, vegye fel őket a **belefoglalási** listába felvenni. Annak érdekében, hogy egy személy a házirend nincs megadva, adja hozzá őket a **kizárása** listához.</span><span class="sxs-lookup"><span data-stu-id="15d0b-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="15d0b-120">További: [hogyan Monitor feltételes hozzáférést biztosító eszközök](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="15d0b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

