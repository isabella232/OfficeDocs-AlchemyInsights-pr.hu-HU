---
title: IOS VPP alkalmazások szabály azonosító 1018 használata
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420486"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="2fcc4-102">IOS VPP-alkalmazások használata</span><span class="sxs-lookup"><span data-stu-id="2fcc4-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="2fcc4-103">Olvassa el a további információt a szolgáltatások, megkötések és lépései [vásárolt Microsoft Intune-vásárlás program iOS alkalmazások kezelése](https://docs.microsoft.com/intune/vpp-apps-ios) az Apple kötet beszerzési Program és a támogatást, akkor a Microsoft Intune használatát.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="2fcc4-104">**Gyakori kérdések:** "A felhasználók számára kiosztott az iOS VPP app, de a telepítés sikertelen volt."</span><span class="sxs-lookup"><span data-stu-id="2fcc4-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="2fcc4-105">Ez akkor fordulhat elő, egyetlen VPP token használata esetén több mobileszközön management szolgáltató között.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="2fcc4-106">VPP tokenek az Apple csak egy szolgáltató használhatók.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="2fcc4-107">Több szolgáltató használt VPP tokent, ha a jogkivonat Intune újra kell feltölteni.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="2fcc4-108">A telepítés is sikertelen lehet, ha létesítmények teljes száma meghaladja a licencek számát.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="2fcc4-109">Használati jelentés a licencek megtekintéséhez nyissa meg az **apps Intune Mobile** \> **App licencek** lapon.</span><span class="sxs-lookup"><span data-stu-id="2fcc4-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="2fcc4-110">Visszanyeréséhez használt licencek, lásd: [cikkben.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="2fcc4-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

