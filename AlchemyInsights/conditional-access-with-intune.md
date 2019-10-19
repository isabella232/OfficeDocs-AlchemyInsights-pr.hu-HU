---
title: Feltételes elérés Intune szolgáltatással
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504996"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c18d5-102">Feltételes elérés Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="c18d5-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c18d5-103">A **feltételes hozzáférés** Intune szolgáltatással 3 lépést igényel:</span><span class="sxs-lookup"><span data-stu-id="c18d5-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="c18d5-104">Hozzon létre egy olyan **feltételes hozzáférési házirendet** , amely meghatározza a védelem alatt álló erőforrásokat, és hogy milyen feltételeknek kell megfelelni az erőforrásokhoz való hozzáféréshez.</span><span class="sxs-lookup"><span data-stu-id="c18d5-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="c18d5-105">Például egy eszköznek kompatibilisnek kell lennie a vállalati e-mail hozzáférés előtt.</span><span class="sxs-lookup"><span data-stu-id="c18d5-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="c18d5-106">A **megfelelőségi házirend** létrehozásával meghatározhatja, hogy mely beállításokat kell teljesíteni ahhoz, hogy az eszköz megfelelőnek minősüljenek.</span><span class="sxs-lookup"><span data-stu-id="c18d5-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c18d5-107">Például egy eszköznek legalább 6 számjegyből álló tüskétnek kell lennie ahhoz, hogy megfeleljen a szabványnak.</span><span class="sxs-lookup"><span data-stu-id="c18d5-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="c18d5-108">A **megfelelőségi házirendek** és a **feltételes hozzáférés házirend** biztosítása a felhasználók kívánt csoportjait célozza.</span><span class="sxs-lookup"><span data-stu-id="c18d5-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="c18d5-109">Ehhez szükség lehet arra, hogy a Azure Active Directoryban a felhasználók meghatározott csoportjait lehessen létrehozni.</span><span class="sxs-lookup"><span data-stu-id="c18d5-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="c18d5-110">Bővebben:</span><span class="sxs-lookup"><span data-stu-id="c18d5-110">Read more:</span></span>
  
- [<span data-ttu-id="c18d5-111">Gyakorlati tanácsok a feltételes hozzáféréshez</span><span class="sxs-lookup"><span data-stu-id="c18d5-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="c18d5-112">Ismerkedés a feltételes hozzáféréssel</span><span class="sxs-lookup"><span data-stu-id="c18d5-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

