---
title: Bizalmasság-címkék automatikus alkalmazása
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1737"
- "9000181"
ms.openlocfilehash: fb05213b7b1efecbabc3e25f6c4587b0d303f783
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707236"
---
# <a name="auto-apply-sensitivity-labels"></a><span data-ttu-id="159f8-102">Bizalmasság-címkék automatikus alkalmazása</span><span class="sxs-lookup"><span data-stu-id="159f8-102">Auto-apply sensitivity labels</span></span>

<span data-ttu-id="159f8-103">A bizalmasság-címkéket a felhasználók manuálisan is alkalmazhatók a tartalomra, vagy beállíthatja, hogy automatikusan alkalmazza őket a tartalomra.</span><span class="sxs-lookup"><span data-stu-id="159f8-103">Sensitivity labels can be manually applied to content by users, or you can configure them to be automatically applied to content.</span></span>

<span data-ttu-id="159f8-104">A bizalmasság-címkék automatikus alkalmazása megszünteti a felhasználóknak a tartalom osztályozásának és a házirendkonfigurációkról való értesítésének a képzését.</span><span class="sxs-lookup"><span data-stu-id="159f8-104">Automatically applying sensitivity labels removes the need to train users on how to classify content and the need to notify them of policy configurations.</span></span>

<span data-ttu-id="159f8-105">A címkék automatikus alkalmazásához az alábbiakra van szükség:</span><span class="sxs-lookup"><span data-stu-id="159f8-105">To apply labels automatically, the following is required:</span></span>

- <span data-ttu-id="159f8-106">Azure Information Protection P2-előfizetés</span><span class="sxs-lookup"><span data-stu-id="159f8-106">Azure Information Protection P2 subscription</span></span>
- [<span data-ttu-id="159f8-107">Az Azure Information Protection egyesített címkézési ügyfélprogram letöltése és telepítése</span><span class="sxs-lookup"><span data-stu-id="159f8-107">Download and install the Azure Information Protection unified labeling client</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

<span data-ttu-id="159f8-108">Dolgozunk azon a natív támogatáson, amelyhez a jövőben nem lesz szükség az Azure Information Protection egyesített címkézési ügyfélalkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="159f8-108">We're working on native support that won't require the Azure Information Protection unified labeling client in the future.</span></span>

<span data-ttu-id="159f8-109">Jelenleg csak a Windows támogatja az egységes címkézési ügyfélprogramot.</span><span class="sxs-lookup"><span data-stu-id="159f8-109">Currently, only Windows supports the unified labeling client.</span></span>  <span data-ttu-id="159f8-110">A funkció még nem támogatott Macen, iOS-en és Androidon.</span><span class="sxs-lookup"><span data-stu-id="159f8-110">The feature is not yet supported on Mac, iOS and Android.</span></span>

<span data-ttu-id="159f8-111">A tartalmi címkékről és azok tartalomra való automatikus alkalmazásával kapcsolatos további információkért lásd:</span><span class="sxs-lookup"><span data-stu-id="159f8-111">For more information on sensitivity labels and applying them automatically to content,  see:</span></span>

- [<span data-ttu-id="159f8-112">A bizalmasság-címkék áttekintése</span><span class="sxs-lookup"><span data-stu-id="159f8-112">Overview of sensitivity labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [<span data-ttu-id="159f8-113">Tartalom automatikus alkalmazása tartalomra</span><span class="sxs-lookup"><span data-stu-id="159f8-113">Apply a sensitivity label to content automatically</span></span>](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically)