---
title: Intune feltételes hozzáférés
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504996"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="dd754-102">Intune feltételes hozzáférés</span><span class="sxs-lookup"><span data-stu-id="dd754-102">Conditional Access with Intune</span></span>

<span data-ttu-id="dd754-103">**A feltételes hozzáférésű** használata Intune 3 lépésből áll:</span><span class="sxs-lookup"><span data-stu-id="dd754-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="dd754-104">Hozzon létre egy **Feltételes házirend** határozza meg, milyen erőforrásokat védett, és feltételeket kell e források eléréséhez kell megfelelni.</span><span class="sxs-lookup"><span data-stu-id="dd754-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="dd754-105">Például egy eszközt kell megfelelő vállalati e-mail megnyitása előtt.</span><span class="sxs-lookup"><span data-stu-id="dd754-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="dd754-106">Hozzon létre egy **Megfelelési házirend** , amely az eszköznek kompatibilisnek minősültek teljesítendő beállítások is megadhatók.</span><span class="sxs-lookup"><span data-stu-id="dd754-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="dd754-107">Például egy eszköznek rendelkeznie kell legalább 6 számjegyű PIN-kód előtt kompatibilis számít.</span><span class="sxs-lookup"><span data-stu-id="dd754-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="dd754-108">**Megfelelés irányelveinek** és a **Feltételes hozzáférési házirendek** a kívánt felhasználói csoportok célzott biztosítása.</span><span class="sxs-lookup"><span data-stu-id="dd754-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="dd754-109">Ehhez néha Azure az Active Directoryban a felhasználók adott csoportjaira létrehozása.</span><span class="sxs-lookup"><span data-stu-id="dd754-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="dd754-110">Tudjon meg többet:</span><span class="sxs-lookup"><span data-stu-id="dd754-110">Read more:</span></span>
  
- [<span data-ttu-id="dd754-111">A feltételes hozzáférés gyakorlati tanácsok</span><span class="sxs-lookup"><span data-stu-id="dd754-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="dd754-112">Bevezetés a feltételes hozzáférést biztosító</span><span class="sxs-lookup"><span data-stu-id="dd754-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

