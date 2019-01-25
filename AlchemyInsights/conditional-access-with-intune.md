---
title: Intune feltételes hozzáférés
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473878"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="0e55e-102">Intune feltételes hozzáférés</span><span class="sxs-lookup"><span data-stu-id="0e55e-102">Conditional Access with Intune</span></span>

<span data-ttu-id="0e55e-103">**A feltételes hozzáférésű** használata Intune 3 lépésből áll:</span><span class="sxs-lookup"><span data-stu-id="0e55e-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="0e55e-p101">Hozzon létre egy **Feltételes házirend** határozza meg, milyen erőforrásokat védett, és feltételeket kell e források eléréséhez kell megfelelni. Például egy eszközt kell megfelelő vállalati e-mail megnyitása előtt.</span><span class="sxs-lookup"><span data-stu-id="0e55e-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="0e55e-p102">Hozzon létre egy **Megfelelési házirend** , amely az eszköznek kompatibilisnek minősültek teljesítendő beállítások is megadhatók. Például egy eszköznek rendelkeznie kell legalább 6 számjegyű PIN-kód előtt kompatibilis számít.</span><span class="sxs-lookup"><span data-stu-id="0e55e-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="0e55e-p103">**Megfelelés irányelveinek** és a **Feltételes hozzáférési házirendek** a kívánt felhasználói csoportok célzott biztosítása. Ehhez néha Azure az Active Directoryban a felhasználók adott csoportjaira létrehozása.</span><span class="sxs-lookup"><span data-stu-id="0e55e-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="0e55e-110">További tudnivalók</span><span class="sxs-lookup"><span data-stu-id="0e55e-110">Read more:</span></span>
  
- [<span data-ttu-id="0e55e-111">A feltételes hozzáférés gyakorlati tanácsok</span><span class="sxs-lookup"><span data-stu-id="0e55e-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="0e55e-112">Bevezetés a feltételes hozzáférést biztosító</span><span class="sxs-lookup"><span data-stu-id="0e55e-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

