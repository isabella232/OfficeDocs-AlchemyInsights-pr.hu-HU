---
title: Feltételes hozzáférés az Intune-nal
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706023"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9e13c-102">Feltételes hozzáférés az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="9e13c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9e13c-103">A **feltételes hozzáférés** intune-nal való használata 3 lépést igényel:</span><span class="sxs-lookup"><span data-stu-id="9e13c-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="9e13c-104">Hozzon létre egy **feltételes hozzáférési szabályzatot,** amely meghatározza, hogy milyen erőforrások at védenek, és milyen feltételeknek kell megfelelni az erőforrások eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="9e13c-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="9e13c-105">Egy eszköznek például megfelelőnek kell lennie a vállalati e-mailek elérése előtt.</span><span class="sxs-lookup"><span data-stu-id="9e13c-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="9e13c-106">Hozzon létre egy **megfelelőségi szabályzatot** olyan beállítások meghatározásához, amelyeket teljesíteni kell ahhoz, hogy az eszköz megfelelőnek minősüljen.</span><span class="sxs-lookup"><span data-stu-id="9e13c-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9e13c-107">Egy eszköznek például legalább 6 számjegyből álló tűvel kell rendelkeznie ahhoz, hogy megfelelőnek minősüljön.</span><span class="sxs-lookup"><span data-stu-id="9e13c-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="9e13c-108">Annak **biztosítása, hogy mind a megfelelőségi szabályzatok,** mind a **feltételes hozzáférési házirendek** a kívánt felhasználói csoportokra irányuljanak.</span><span class="sxs-lookup"><span data-stu-id="9e13c-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="9e13c-109">Ez szükség lehet a felhasználók adott csoportjainak az Azure Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="9e13c-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="9e13c-110">Bővebben:</span><span class="sxs-lookup"><span data-stu-id="9e13c-110">Read more:</span></span>
  
- [<span data-ttu-id="9e13c-111">A feltételes hozzáféréssel kapcsolatos gyakorlati tanácsok</span><span class="sxs-lookup"><span data-stu-id="9e13c-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="9e13c-112">A feltételes hozzáférés – első lépések</span><span class="sxs-lookup"><span data-stu-id="9e13c-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

