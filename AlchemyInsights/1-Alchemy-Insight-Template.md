---
title: ugyanaz, mint a fájlnév a legcélszerűbb
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
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683851"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="f90a0-102">Szükséges Alkímia fej H1, H2 meg nem működnek.</span><span class="sxs-lookup"><span data-stu-id="f90a0-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="f90a0-103">Gyakorlati tanácsokat és iránymutatásokat Alkímia szerzői:</span><span class="sxs-lookup"><span data-stu-id="f90a0-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="f90a0-104">**Nem ágyazódnak egymásba Alkímia elképzelések mappákban**- Ezzel megszünteti az URL-szerkezet.</span><span class="sxs-lookup"><span data-stu-id="f90a0-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="f90a0-105">Azt történő rögzítésének a keresést.</span><span class="sxs-lookup"><span data-stu-id="f90a0-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="f90a0-106">A **AlchemyInsights** mappában található fájlok kisbetűs fájlnevek ex tereket kötőjellel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="f90a0-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="f90a0-107">***how-to-enable-per-tartás***.</span><span class="sxs-lookup"><span data-stu-id="f90a0-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="f90a0-108">Az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net) Szabályazonosító vagy hibasor Azonosítóját tartalmazza a ms.custom mezőben.</span><span class="sxs-lookup"><span data-stu-id="f90a0-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="f90a0-109">ex.</span><span class="sxs-lookup"><span data-stu-id="f90a0-109">ex.</span></span> <span data-ttu-id="f90a0-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="f90a0-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="f90a0-111">A sablonként használni a metaadatokat a többi fájl tetején.</span><span class="sxs-lookup"><span data-stu-id="f90a0-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="f90a0-112">Az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net)keresse meg a szakasz le **vevő-Insight címe:** és a betekintést a H1 címe, amely a kiindulási pont használatát.</span><span class="sxs-lookup"><span data-stu-id="f90a0-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="f90a0-113">Alkímia ismereteknek kell csak egyetlen H1 tetején vagy azok gyártási megszakad.</span><span class="sxs-lookup"><span data-stu-id="f90a0-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="f90a0-114">H2s nem teszik, így használata **félkövér** vagy más egyezmények külön szakaszokban jeléül.</span><span class="sxs-lookup"><span data-stu-id="f90a0-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="f90a0-115">Ezután töltse ki a szövegtörzs, az Alkímia szabály lap vevő elképzelések részében a tervezet anyag használata</span><span class="sxs-lookup"><span data-stu-id="f90a0-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="f90a0-116">Felsorolásjeles listák rendben.</span><span class="sxs-lookup"><span data-stu-id="f90a0-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="f90a0-117">Számozott listák túl</span><span class="sxs-lookup"><span data-stu-id="f90a0-117">Numbered lists too</span></span>
    1. <span data-ttu-id="f90a0-118">**Félkövér** és *dőlt* a-ok</span><span class="sxs-lookup"><span data-stu-id="f90a0-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="f90a0-119">Hivatkozások mindig kell lennie, vagy **"webes hivatkozásokat" / külső** vagy **felhasználói felületének elemeit mély kapcsolatokat**, nem belső hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="f90a0-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="f90a0-120">Képek nem hivatalosan támogatott most, de szerepel az ütemtervben.</span><span class="sxs-lookup"><span data-stu-id="f90a0-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="f90a0-121">És ez már valóban egy kicsit túl hosszú.</span><span class="sxs-lookup"><span data-stu-id="f90a0-121">And this is really already a bit too long.</span></span> <span data-ttu-id="f90a0-122">Legjobb gyakorlat az, körülbelül 400 karakter---</span><span class="sxs-lookup"><span data-stu-id="f90a0-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="f90a0-123">Ha készen áll a tartalom, húzza a élő ágat.</span><span class="sxs-lookup"><span data-stu-id="f90a0-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="f90a0-124">Ezután menjen az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net) , és írja be a fájlnevet az URL-cím mezőben.</span><span class="sxs-lookup"><span data-stu-id="f90a0-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="f90a0-125">M</span><span class="sxs-lookup"><span data-stu-id="f90a0-125">M</span></span>