---
title: ugyanaz mint filenév van legjobb
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800047"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0c686-102">Kötelező Alchemy fejléc H1, H2's nem működik.</span><span class="sxs-lookup"><span data-stu-id="0c686-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="0c686-103">A legjobb gyakorlatok és iránymutatások Alchemy authoring:</span><span class="sxs-lookup"><span data-stu-id="0c686-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0c686-104">Ne **fészkel alkímia Insights a mappák**-Ez megtöri az URL struktúrát.</span><span class="sxs-lookup"><span data-stu-id="0c686-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="0c686-105">Mi vagyunk látszó-ba rögzítő ez.</span><span class="sxs-lookup"><span data-stu-id="0c686-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="0c686-106">Az **Alchemyinsights** mappában lévő fájloknak kisbetűs fájlnevekkel kell rendelkezniük, a szóközök pl. kötőjelet kell tükrözniük.</span><span class="sxs-lookup"><span data-stu-id="0c686-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="0c686-107">***hogyan kell-Enable-perek-Hold***.</span><span class="sxs-lookup"><span data-stu-id="0c686-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="0c686-108">A Rule ID, vagy a Bucket ID azonosítót az [alkímia partner portálja](https://alchemyportal.azurewebsites.net) tartalmazza a MS. Custom mezőben.</span><span class="sxs-lookup"><span data-stu-id="0c686-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="0c686-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="0c686-109">ex.</span></span> <span data-ttu-id="0c686-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="0c686-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="0c686-111">Sablonként használhatja a fájl tetején lévő többi metaadatot.</span><span class="sxs-lookup"><span data-stu-id="0c686-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="0c686-112">Az [alkímia partner portálon](https://alchemyportal.azurewebsites.net), navigálni le a szakaszt **ügyfél Insight cím:** és használni, hogy a kiindulási pont a H1 címét a betekintést.</span><span class="sxs-lookup"><span data-stu-id="0c686-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0c686-113">Alchemy Insights kell lennie csak egy H1 a tetején, vagy fognak törni a termelést.</span><span class="sxs-lookup"><span data-stu-id="0c686-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="0c686-114">H2s nem teszik sem így használja **merész** vagy más egyezmények jelzi külön szakaszok.</span><span class="sxs-lookup"><span data-stu-id="0c686-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0c686-115">Következő, töltse ki a szövegtörzs segítségével a tervezet anyagot az ügyfél Insights szakaszában az alkímia szabály oldal</span><span class="sxs-lookup"><span data-stu-id="0c686-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0c686-116">A felsorolásjeles listák jól</span><span class="sxs-lookup"><span data-stu-id="0c686-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0c686-117">Számozott listák is</span><span class="sxs-lookup"><span data-stu-id="0c686-117">Numbered lists too</span></span>
    1. <span data-ttu-id="0c686-118">**Félkövér** és *dőlt* is a-ok</span><span class="sxs-lookup"><span data-stu-id="0c686-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0c686-119">Linkek mindig vagy **"linkeket web"/külső** vagy **mély-linkek UI elemek**, nem a belső linkek.</span><span class="sxs-lookup"><span data-stu-id="0c686-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="0c686-120">Képek nem hivatalosan támogatott ebben az időben, de ez az ütemterv.</span><span class="sxs-lookup"><span data-stu-id="0c686-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="0c686-121">És ez tényleg már egy kicsit túl hosszú.</span><span class="sxs-lookup"><span data-stu-id="0c686-121">And this is really already a bit too long.</span></span> <span data-ttu-id="0c686-122">A legjobb gyakorlat mintegy 400 karakter---------------------------------</span><span class="sxs-lookup"><span data-stu-id="0c686-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0c686-123">Egyszer-a elégedett van kész, húz ez-hoz él ág.</span><span class="sxs-lookup"><span data-stu-id="0c686-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="0c686-124">Ezután menj az [alkímia partner portálra](https://alchemyportal.azurewebsites.net) és írd be a fájlnevet az URL mezőbe.</span><span class="sxs-lookup"><span data-stu-id="0c686-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 