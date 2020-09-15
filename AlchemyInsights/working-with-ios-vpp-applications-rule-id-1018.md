---
title: Az iOS VPP-alkalmazásokkal végzett műveletek szabály-azonosítója 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688948"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="6a490-102">Az iOS VPP-alkalmazásokkal végezhető műveletek</span><span class="sxs-lookup"><span data-stu-id="6a490-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="6a490-103">A cikkből megtudhatja, [hogy miként kezelheti a mennyiségi vásárlással vásárolt iOS-alkalmazásokat a Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) segítségével, és megismerheti a Microsoft Intune szolgáltatásban elérhető Apple mennyiségi vásárlási program és a támogatás funkcióit.</span><span class="sxs-lookup"><span data-stu-id="6a490-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="6a490-104">**Gyakori problémák:** "Egy iOS VPP alkalmazást Rendeltem a felhasználóknak, de a telepítés nem sikerült."</span><span class="sxs-lookup"><span data-stu-id="6a490-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="6a490-105">Ez akkor fordulhat elő, ha egyetlen VPP-tokent használ több mobileszköz-kezelési szolgáltatónál.</span><span class="sxs-lookup"><span data-stu-id="6a490-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="6a490-106">Az Apple-ből származó VPP-tokenek csak egy szolgáltatónál használhatók.</span><span class="sxs-lookup"><span data-stu-id="6a490-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="6a490-107">Ha egy VPP-tokent több szolgáltatónál használt, újra fel kell töltenie a jogkivonatot a Intune-ra.</span><span class="sxs-lookup"><span data-stu-id="6a490-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="6a490-108">A telepítés akkor is meghiúsulhat, ha a telepített példányok száma túllépi a licencek számát.</span><span class="sxs-lookup"><span data-stu-id="6a490-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="6a490-109">A licencek használati jelentésének megtekintéséhez nyissa meg az **Intune Mobile apps** \> **app licencek** lapját.</span><span class="sxs-lookup"><span data-stu-id="6a490-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="6a490-110">Ha meg szeretné tudni, hogy miként állíthatja vissza a licenceket a használatban, olvassa el [ezt a cikket.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="6a490-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
