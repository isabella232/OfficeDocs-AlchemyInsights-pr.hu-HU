---
title: ugyanaz, mint a fájlnév a legjobb
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664136"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="867b7-102">"A kötelező alkímia fejléce, a H2's nem működik."</span><span class="sxs-lookup"><span data-stu-id="867b7-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="867b7-103">Ajánlott eljárások és útmutatók az alkímia szerkesztéséhez:</span><span class="sxs-lookup"><span data-stu-id="867b7-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="867b7-104">Ne **ágyazza be az Alchemy**-elemzéseket a mappákba – Ez megtöri az URL-struktúrát.</span><span class="sxs-lookup"><span data-stu-id="867b7-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="867b7-105">Ebben a cikkben keresünk.</span><span class="sxs-lookup"><span data-stu-id="867b7-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="867b7-106">A **AlchemyInsights** mappában lévő fájloknak kisbetűs fájlnevet kell használniuk az ex szóköz billentyűkombinációval.</span><span class="sxs-lookup"><span data-stu-id="867b7-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="867b7-107">***útmutató – engedélyezés – peres eljárás***</span><span class="sxs-lookup"><span data-stu-id="867b7-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="867b7-108">Adja meg a szabály AZONOSÍTÓját vagy a vödör AZONOSÍTÓját az [Alchemy partner portálról](https://alchemyportal.azurewebsites.net) a MS. egyéni mezőben.</span><span class="sxs-lookup"><span data-stu-id="867b7-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="867b7-109">ex.</span><span class="sxs-lookup"><span data-stu-id="867b7-109">ex.</span></span> <span data-ttu-id="867b7-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="867b7-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="867b7-111">Használja a fájl felső részén található metaadatokat sablonként.</span><span class="sxs-lookup"><span data-stu-id="867b7-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="867b7-112">Az [Alchemy partner portálon](https://alchemyportal.azurewebsites.net)lépjen lefelé az **ügyfél-betekintési cím** mezőbe, és használja azt kiindulási pontként az Insight-címéhez.</span><span class="sxs-lookup"><span data-stu-id="867b7-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="867b7-113">Az alkímiai elemzéseknek csak egy H1-nek kell lenniük a tetején, vagy a termelésben szünetük lesz.</span><span class="sxs-lookup"><span data-stu-id="867b7-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="867b7-114">A H2s nem jeleníti meg a **félkövér** vagy más konvenciókat, hogy külön szakaszt adjon meg.</span><span class="sxs-lookup"><span data-stu-id="867b7-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="867b7-115">Ezután töltse ki a szövegtörzset az Alchemy szabály lapjának ügyfél-betekintési részén található anyag segítségével.</span><span class="sxs-lookup"><span data-stu-id="867b7-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="867b7-116">A listajeles felsorolások jól láthatók</span><span class="sxs-lookup"><span data-stu-id="867b7-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="867b7-117">Számozott listák</span><span class="sxs-lookup"><span data-stu-id="867b7-117">Numbered lists too</span></span>
    1. <span data-ttu-id="867b7-118">A **félkövér** és a *dőlt* a-ok</span><span class="sxs-lookup"><span data-stu-id="867b7-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="867b7-119">A hivatkozásoknak mindig a **"hivatkozások a webre"/External** kell lenniük, vagy **mély hivatkozásokat kell használniuk a felhasználóifelület-elemekre, nem pedig a**belső hivatkozásokra.</span><span class="sxs-lookup"><span data-stu-id="867b7-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="867b7-120">Jelenleg a képek jelenleg nem támogatottak, de az ütemterven van.</span><span class="sxs-lookup"><span data-stu-id="867b7-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="867b7-121">És ez már egy kicsit túl hosszú.</span><span class="sxs-lookup"><span data-stu-id="867b7-121">And this is really already a bit too long.</span></span> <span data-ttu-id="867b7-122">A helyes gyakorlat a 400 karakterekről szól---------------------------------</span><span class="sxs-lookup"><span data-stu-id="867b7-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="867b7-123">Miután elkészült a tartalom, húzza azt az aktív ágra.</span><span class="sxs-lookup"><span data-stu-id="867b7-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="867b7-124">Ezután nyissa meg az [Alchemy Partner portált](https://alchemyportal.azurewebsites.net) , és írja be a fájlnevet az URL-mezőbe.</span><span class="sxs-lookup"><span data-stu-id="867b7-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 