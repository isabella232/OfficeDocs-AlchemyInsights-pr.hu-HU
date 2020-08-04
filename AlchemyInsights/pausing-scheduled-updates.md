---
title: Ütemezett frissítések szüneteltetése
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555509"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="b5e16-102">Ütemezett frissítések szüneteltetése</span><span class="sxs-lookup"><span data-stu-id="b5e16-102">Pausing scheduled updates</span></span>

<span data-ttu-id="b5e16-103">Szüneteltetési parancs kiadásakor az eszközök csak az Intune következő bejelentkezésekekénél dolgozzák fel a parancsot.</span><span class="sxs-lookup"><span data-stu-id="b5e16-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="b5e16-104">Emiatt az eszközök a következőkkel rendelkezhetnek:</span><span class="sxs-lookup"><span data-stu-id="b5e16-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="b5e16-105">A bejelentkezés előtt telepítette az ütemezett frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="b5e16-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="b5e16-106">A szüneteltetési parancs kiadásakor ki van kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="b5e16-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="b5e16-107">Ebben az esetben, amikor az eszközök be voltak kapcsolva, előfordulhat, hogy a bejelentkezés előtt letöltötték és telepítették az ütemezett frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="b5e16-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>