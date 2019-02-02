---
title: 'ugyanaz, mint a legcélszerűbb fájlnév [szabály #-leírás]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697132"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="cc907-102">Szükséges Alkímia fej H1, H2 meg nem működnek.</span><span class="sxs-lookup"><span data-stu-id="cc907-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="cc907-103">Gyakorlati tanácsokat és iránymutatásokat Alkímia szerzői:</span><span class="sxs-lookup"><span data-stu-id="cc907-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="cc907-p101">**Nem ágyazódnak egymásba Alkímia elképzelések mappákban**- Ezzel megszünteti az URL-szerkezet. Azt történő rögzítésének a keresést.</span><span class="sxs-lookup"><span data-stu-id="cc907-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="cc907-106">A **AlchemyInsights** mappában található fájlokat kell Szabályazonosító és az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net) szabály nevét a fájlnév.</span><span class="sxs-lookup"><span data-stu-id="cc907-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="cc907-p102">például ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="cc907-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="cc907-p103">A sablonként használni a metaadatokat a fájl elején. Semmi másra nincs szükség.</span><span class="sxs-lookup"><span data-stu-id="cc907-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="cc907-111">Az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net)keresse meg a szakasz le **vevő-Insight címe:** és a betekintést a H1 címe, amely a kiindulási pont használatát.</span><span class="sxs-lookup"><span data-stu-id="cc907-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="cc907-p104">Alkímia ismereteknek kell csak egyetlen H1 tetején vagy azok gyártási megszakad. H2s nem teszik, így használata **félkövér** vagy más egyezmények külön szakaszokban jeléül.</span><span class="sxs-lookup"><span data-stu-id="cc907-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="cc907-114">Ezután töltse ki a szövegtörzs, az Alkímia szabály lap vevő elképzelések részében a tervezet anyag használata</span><span class="sxs-lookup"><span data-stu-id="cc907-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="cc907-115">Felsorolásjeles listák rendben.</span><span class="sxs-lookup"><span data-stu-id="cc907-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="cc907-116">Számozott listák túl</span><span class="sxs-lookup"><span data-stu-id="cc907-116">Numbered lists too</span></span>
    1. <span data-ttu-id="cc907-117">**Félkövér** és *dőlt* a-ok</span><span class="sxs-lookup"><span data-stu-id="cc907-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="cc907-118">Hivatkozások mindig kell lennie, vagy **"webes hivatkozásokat" / külső** vagy **felhasználói felületének elemeit mély kapcsolatokat**, nem belső hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="cc907-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="cc907-p105">És ez már valóban egy kicsit túl hosszú. Legjobb gyakorlat az, körülbelül 400 karakter---</span><span class="sxs-lookup"><span data-stu-id="cc907-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="cc907-p106">Ha készen áll a tartalom, húzza a élő ágat. Ezután menjen az [Alkímia Partner portal](https://alchemyportal.azurewebsites.net) , és írja be a fájlnevet az URL-cím mezőben. Ellenőrizze, hogy felülvizsgálják, és közzé Insight szerint "Igen", és kattintson a frissítés szabály. **(Ez fog megjelenni a portál - hamarosan felszabadítása az új verzió a prettier.)** 
 ![URL-mező](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="cc907-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

