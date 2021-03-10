---
title: A meglévő böngészőkörnyezet értékelése és a célok meghatározása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693640"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="48ebf-102">A meglévő böngészőkörnyezet értékelése és a célok meghatározása</span><span class="sxs-lookup"><span data-stu-id="48ebf-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="48ebf-103">A böngésző jelenlegi állapotának és a projektlátásnak a segítségével biztosíthatja, hogy a projekt minden érintettje egy vonalban van, és ugyanazon cél érdekében dolgoznak.</span><span class="sxs-lookup"><span data-stu-id="48ebf-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="48ebf-104">Hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="48ebf-104">Follow these steps:</span></span>

1. <span data-ttu-id="48ebf-105">Határozza meg az aktuális állapotot.</span><span class="sxs-lookup"><span data-stu-id="48ebf-105">Define your current state.</span></span> <span data-ttu-id="48ebf-106">Célszerű megemlíteni az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="48ebf-106">Consider the following:</span></span>
- <span data-ttu-id="48ebf-107">Jelenleg mely böngészők vannak telepítve a környezetében?</span><span class="sxs-lookup"><span data-stu-id="48ebf-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="48ebf-108">Melyik böngésző van beállítva alapértelmezett böngészőként?</span><span class="sxs-lookup"><span data-stu-id="48ebf-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="48ebf-109">Szüksége van az Internet Explorerre néhány alkalmazáshoz?</span><span class="sxs-lookup"><span data-stu-id="48ebf-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="48ebf-110">Vállalati módú webhelylistát használ az Internet Explorer beállításához?</span><span class="sxs-lookup"><span data-stu-id="48ebf-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="48ebf-111">Mely operációs rendszerek (például a Windows 10 és a macOS) támogatottak a környezetében?</span><span class="sxs-lookup"><span data-stu-id="48ebf-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="48ebf-112">Milyen kezelőeszközöket használ a böngésző kezeléséhez?</span><span class="sxs-lookup"><span data-stu-id="48ebf-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="48ebf-113">Ki a felelős a böngészők konfigurációáért és kezeléséért?</span><span class="sxs-lookup"><span data-stu-id="48ebf-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="48ebf-114">Milyen folyamattal érvényesíthető a böngészőkompatibilitás?</span><span class="sxs-lookup"><span data-stu-id="48ebf-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="48ebf-115">Határozza meg a telepítés céljait.</span><span class="sxs-lookup"><span data-stu-id="48ebf-115">Define the goals for your deployment.</span></span> <span data-ttu-id="48ebf-116">Tartsa szem előtt az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="48ebf-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="48ebf-117">Be szeretné állítani a [Microsoft Edge-et alapértelmezett böngészőként?](https://docs.microsoft.com/DeployEdge/edge-default-browser)</span><span class="sxs-lookup"><span data-stu-id="48ebf-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="48ebf-118">Szeretné elrejteni a Microsoft Edge régi verzióját, vagy elérhetővé szeretné tenni a [felhasználóknak?](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)</span><span class="sxs-lookup"><span data-stu-id="48ebf-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="48ebf-119">Hogyan fogja [konfigurálni a Microsoft Edge-et?](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)</span><span class="sxs-lookup"><span data-stu-id="48ebf-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="48ebf-120">Milyen funkciókat kell konfigurálni a kezdeti telepítés részeként?</span><span class="sxs-lookup"><span data-stu-id="48ebf-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="48ebf-121">Milyen folyamat során történik az azonosított kompatibilitási vagy konfigurációs problémák megoldása?</span><span class="sxs-lookup"><span data-stu-id="48ebf-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="48ebf-122">A funkciók használatának előfeltételei, például:</span><span class="sxs-lookup"><span data-stu-id="48ebf-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="48ebf-123">Windows Defender alkalmazásőr</span><span class="sxs-lookup"><span data-stu-id="48ebf-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="48ebf-124">Internet Explorer mód</span><span class="sxs-lookup"><span data-stu-id="48ebf-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="48ebf-125">Hitelesítés és szinkronizálás</span><span class="sxs-lookup"><span data-stu-id="48ebf-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="48ebf-126">A lépések végrehajtása után készen áll az üzembe helyezési stratégia megtervezésére.</span><span class="sxs-lookup"><span data-stu-id="48ebf-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
