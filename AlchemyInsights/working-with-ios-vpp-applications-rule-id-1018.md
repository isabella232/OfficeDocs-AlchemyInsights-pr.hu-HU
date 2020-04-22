---
title: Az iOS VPP-alkalmazások 1018-as szabályának alkalmazása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719959"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="4da54-102">Az iOS VPP-alkalmazások kal való együttműködés</span><span class="sxs-lookup"><span data-stu-id="4da54-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="4da54-103">Olvassa [el A Microsoft Intune-nal egy mennyiségi vásárlási program keretében vásárolt iOS-alkalmazások kezelése](https://docs.microsoft.com/intune/vpp-apps-ios) című, a Microsoft Intune-ban található funkciók, korlátozások és az Apple mennyiségi vásárlási programjának használatának lépéseit és a Microsoft Intune-ban nyújtott támogatás használatát.</span><span class="sxs-lookup"><span data-stu-id="4da54-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="4da54-104">**Gyakori problémák:** "IOS VPP alkalmazást rendeltem a felhasználókhoz, de a telepítés nem sikerült."</span><span class="sxs-lookup"><span data-stu-id="4da54-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="4da54-105">Ez akkor fordulhat elő, ha egyetlen VPP-jogkivonatot használ több mobileszköz-felügyeleti szolgáltató között.</span><span class="sxs-lookup"><span data-stu-id="4da54-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="4da54-106">Az Apple VPP-tokenjeit csak egy szolgáltatónál lehet használni.</span><span class="sxs-lookup"><span data-stu-id="4da54-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="4da54-107">Ha több szolgáltatóval használt VPP-jogkivonatot, újra fel kell töltenie a jogkivonatot az Intune-ba.</span><span class="sxs-lookup"><span data-stu-id="4da54-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="4da54-108">A telepítés akkor is sikertelen lehet, ha a telepítések száma meghaladja a licencek számát.</span><span class="sxs-lookup"><span data-stu-id="4da54-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="4da54-109">A licencek használati jelentésének megtekintéséhez nyissa meg az **Intune Mobile apps** \> **alkalmazáslicencek lapját.**</span><span class="sxs-lookup"><span data-stu-id="4da54-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="4da54-110">A használatban lévő licencek visszaigénylésének módjáról [ebben a cikkben olvashat.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="4da54-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
