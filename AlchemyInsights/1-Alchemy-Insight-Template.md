---
title: 'ugyanaz, mint a legcélszerűbb fájlnév [szabály #-leírás]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634506"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="f180a-102">Szükséges Alkímia fej H1, H2 meg nem működnek.</span><span class="sxs-lookup"><span data-stu-id="f180a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="f180a-103">Gyakorlati tanácsokat és iránymutatásokat Alkímia szerzői:</span><span class="sxs-lookup"><span data-stu-id="f180a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="f180a-104">**Nem ágyazódnak egymásba Alkímia elképzelések mappákban**- Ezzel megszünteti az URL-szerkezet.</span><span class="sxs-lookup"><span data-stu-id="f180a-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="f180a-105">Azt történő rögzítésének a keresést.</span><span class="sxs-lookup"><span data-stu-id="f180a-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="f180a-106">A **AlchemyInsights** mappában található fájlokat kell Szabályazonosító és az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net) szabály nevét a fájlnév.</span><span class="sxs-lookup"><span data-stu-id="f180a-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="f180a-107">ex.</span><span class="sxs-lookup"><span data-stu-id="f180a-107">ex.</span></span> <span data-ttu-id="f180a-108">***976-How-to-enable-litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="f180a-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="f180a-109">A sablonként használni a metaadatokat a fájl elején.</span><span class="sxs-lookup"><span data-stu-id="f180a-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="f180a-110">Semmi másra nincs szükség.</span><span class="sxs-lookup"><span data-stu-id="f180a-110">Nothing else is required.</span></span>
1. <span data-ttu-id="f180a-111">Az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net)keresse meg a szakasz le **vevő-Insight címe:** és a betekintést a H1 címe, amely a kiindulási pont használatát.</span><span class="sxs-lookup"><span data-stu-id="f180a-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="f180a-112">Alkímia ismereteknek kell csak egyetlen H1 tetején vagy azok gyártási megszakad.</span><span class="sxs-lookup"><span data-stu-id="f180a-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="f180a-113">H2s nem teszik, így használata **félkövér** vagy más egyezmények külön szakaszokban jeléül.</span><span class="sxs-lookup"><span data-stu-id="f180a-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="f180a-114">Ezután töltse ki a szövegtörzs, az Alkímia szabály lap vevő elképzelések részében a tervezet anyag használata</span><span class="sxs-lookup"><span data-stu-id="f180a-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="f180a-115">Felsorolásjeles listák rendben.</span><span class="sxs-lookup"><span data-stu-id="f180a-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="f180a-116">Számozott listák túl</span><span class="sxs-lookup"><span data-stu-id="f180a-116">Numbered lists too</span></span>
    1. <span data-ttu-id="f180a-117">**Félkövér** és *dőlt* a-ok</span><span class="sxs-lookup"><span data-stu-id="f180a-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="f180a-118">Hivatkozások mindig kell lennie, vagy **"webes hivatkozásokat" / külső** vagy **felhasználói felületének elemeit mély kapcsolatokat**, nem belső hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="f180a-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="f180a-119">És ez már valóban egy kicsit túl hosszú.</span><span class="sxs-lookup"><span data-stu-id="f180a-119">And this is really already a bit too long.</span></span> <span data-ttu-id="f180a-120">Legjobb gyakorlat az, körülbelül 400 karakter---</span><span class="sxs-lookup"><span data-stu-id="f180a-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="f180a-121">Ha készen áll a tartalom, húzza a élő ágat.</span><span class="sxs-lookup"><span data-stu-id="f180a-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="f180a-122">Ezután menjen az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net) , és írja be a fájlnevet az URL-cím mezőben.</span><span class="sxs-lookup"><span data-stu-id="f180a-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="f180a-123">Ellenőrizze, hogy felülvizsgálják, és közzé Insight szerint "Igen", és kattintson a frissítés szabály.</span><span class="sxs-lookup"><span data-stu-id="f180a-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="f180a-124">**(Ez fog megjelenni a portál - hamarosan felszabadítása az új verzió a prettier.)** 
 ![URL-mező](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="f180a-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

