---
title: ugyanaz, mint a fájlnév a legjobb
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750972"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="02b54-102">"Szükséges Alkímia Fejléc H1, H2's nem működik."</span><span class="sxs-lookup"><span data-stu-id="02b54-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="02b54-103">Gyakorlati tanácsok és irányelvek az alkímia iméniai szerkesztéshez:</span><span class="sxs-lookup"><span data-stu-id="02b54-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="02b54-104">**Ne ágyazd be az Alchemy Insights-ot a mappákba**- ez megtöri az URL-struktúrát.</span><span class="sxs-lookup"><span data-stu-id="02b54-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="02b54-105">Ezt meg akarjuk javítani.</span><span class="sxs-lookup"><span data-stu-id="02b54-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="02b54-106">Az **AlchemyInsights** mappában lévő fájloknak kisbetűs fájlnevekkel kell rendelkezniük, kötőjelekkel az ex szóközökhöz.</span><span class="sxs-lookup"><span data-stu-id="02b54-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="02b54-107">***hogyan lehet engedélyezni a peres eljárásokat.***</span><span class="sxs-lookup"><span data-stu-id="02b54-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="02b54-108">Adja meg a szabályazonosítót vagy a gyűjtőazonosítót az [Alkímiapartner portálról](https://alchemyportal.azurewebsites.net) az ms.custom mezőben.</span><span class="sxs-lookup"><span data-stu-id="02b54-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="02b54-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="02b54-109">ex.</span></span> <span data-ttu-id="02b54-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="02b54-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="02b54-111">Sablonként használja a fájl tetején lévő többi metaadatot.</span><span class="sxs-lookup"><span data-stu-id="02b54-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="02b54-112">Az [Alkímia partner portálján](https://alchemyportal.azurewebsites.net)keresse le az **Ügyfél betekintési címe szakaszt,** és használja ezt a H1 cím kiindulópontjaként az elemzéshez.</span><span class="sxs-lookup"><span data-stu-id="02b54-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="02b54-113">Alchemy Insights kell csak egy H1 a tetején, vagy azok szünet a termelésben.</span><span class="sxs-lookup"><span data-stu-id="02b54-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="02b54-114">A H2s nem teszi kitévá az okat, ezért **használjon félkövér** vagy más konvenciókat a különálló szakaszok jelzéséhez.</span><span class="sxs-lookup"><span data-stu-id="02b54-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="02b54-115">Ezután töltse ki a törzsszöveget az Alkímiai szabály lap Customer Insights szakaszában található vázlat anyag használatával.</span><span class="sxs-lookup"><span data-stu-id="02b54-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="02b54-116">A listajeles listák rendben vannak</span><span class="sxs-lookup"><span data-stu-id="02b54-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="02b54-117">Számozott listák is</span><span class="sxs-lookup"><span data-stu-id="02b54-117">Numbered lists too</span></span>
    1. <span data-ttu-id="02b54-118">**Merész** és *dőlt* a-ok</span><span class="sxs-lookup"><span data-stu-id="02b54-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="02b54-119">Linkek mindig vagy **"linkeket web"/ külső** VAGY **mély-linkeket ui elemek**, nem belső linkek.</span><span class="sxs-lookup"><span data-stu-id="02b54-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="02b54-120">A képek hivatalosan nem támogatottak jelenleg, de az ütemtervben szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="02b54-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="02b54-121">És ez már így is egy kicsit túl hosszú.</span><span class="sxs-lookup"><span data-stu-id="02b54-121">And this is really already a bit too long.</span></span> <span data-ttu-id="02b54-122">Az ajánlott eljárás körülbelül 400 karakter ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="02b54-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="02b54-123">Ha a tartalom készen áll, húzza ki az élő ágba.</span><span class="sxs-lookup"><span data-stu-id="02b54-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="02b54-124">Ezután nyissa meg az [Alchemy Partner portált,](https://alchemyportal.azurewebsites.net) és írja be a fájlnevet az URL mezőbe.</span><span class="sxs-lookup"><span data-stu-id="02b54-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 