---
title: Webhelyfeltárás
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
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693486"
---
# <a name="do-site-discovery"></a><span data-ttu-id="e589d-102">Webhelyfeltárás</span><span class="sxs-lookup"><span data-stu-id="e589d-102">Do site discovery</span></span>

<span data-ttu-id="e589d-103">Ha a szervezete továbbra is régi webalkalmazásokat használ, és az Internet Explorer módot tervezi használni (amelyet a legtöbb ügyfél használ), akkor további webhelyfeltárási lehetőségeket kell használnia.</span><span class="sxs-lookup"><span data-stu-id="e589d-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="e589d-104">**Már telepítette a Microsoft Edge egy régebbi verzióját**</span><span class="sxs-lookup"><span data-stu-id="e589d-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="e589d-105">Ha már beállította a vállalati webhelylistát a Microsoft Edge régi verziójának megfelelőre, akkor a webhelyfeltárás már majdnem kész.</span><span class="sxs-lookup"><span data-stu-id="e589d-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="e589d-106">Az egyetlen dolog, amit érdemes lehet megtennie, hogy semleges webhelyeket ad hozzá.</span><span class="sxs-lookup"><span data-stu-id="e589d-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="e589d-107">A semleges webhelyek általában egyszeri bejelentkezést biztosítanak.</span><span class="sxs-lookup"><span data-stu-id="e589d-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="e589d-108">Ha a Microsoft Edge-től egy semleges webhelyre kerül, a hitelesítéshez a Microsoft Edge-ben szeretne maradni.</span><span class="sxs-lookup"><span data-stu-id="e589d-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="e589d-109">Ha az Internet Explorer módban semleges webhelyre vált, a hitelesítéshez az Internet Explorer módban szeretne maradni.</span><span class="sxs-lookup"><span data-stu-id="e589d-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="e589d-110">Azonosítsa az Ön által használt SSO- vagy egyéb semleges webhelyeket, és vegye fel őket a vállalati webhelylistára.</span><span class="sxs-lookup"><span data-stu-id="e589d-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="e589d-111">**Az Internet Explorer az alapértelmezett böngésző**</span><span class="sxs-lookup"><span data-stu-id="e589d-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="e589d-112">Ha most csak az Internet Explorert használja, nem biztos, hogy tudja, hogy mely webhelyek frissítettek modern webes szabványokra, és melyekhez még szükség van az Internet Explorerre.</span><span class="sxs-lookup"><span data-stu-id="e589d-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="e589d-113">Ezeket a webhelyeket meg kell találnia, és hozzá kell adnia a vállalati webhelylistához, hogy csak az ilyen webhelyekhez tudja használni az Internet Explorer módot.</span><span class="sxs-lookup"><span data-stu-id="e589d-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="e589d-114">[A Vállalati webhelyfeltárás](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) feltárja az Internet Explorer módra esetleg szüksége lehet a webhelyeket.</span><span class="sxs-lookup"><span data-stu-id="e589d-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="e589d-115">Adatokat gyűjthet Windows Internet Explorer 8–Internet Explorer 11 rendszerű számítógépeken Windows 10, Windows 8.1 vagy Windows 7 rendszeren.</span><span class="sxs-lookup"><span data-stu-id="e589d-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="e589d-116">**Az adatok elemzése**</span><span class="sxs-lookup"><span data-stu-id="e589d-116">**Analyze the data**</span></span>

<span data-ttu-id="e589d-117">Miután összegyűjtötte a webhelyadatokat, az adatok elemzéséhez az alábbi négylépéses eljárást javasoljuk:</span><span class="sxs-lookup"><span data-stu-id="e589d-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="e589d-118">Rendezheti az adatokat tartomány, majd URL-cím szerint.</span><span class="sxs-lookup"><span data-stu-id="e589d-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="e589d-119">Adja meg az Internet Explorer módban konfigurálni szükséges alkalmazáshatárokat.</span><span class="sxs-lookup"><span data-stu-id="e589d-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="e589d-120">Az appot definiáló összes webhelyet és webes vezérlőt fel szeretné azonbanni, de nem szeretne további webhelyeket és vezérlőket tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="e589d-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="e589d-121">Egyes webhelyek lehetnek olyan egyszerűek, mint amikor mások több webhely és lap *https://contoso.com/app1* definiálását követelik meg.</span><span class="sxs-lookup"><span data-stu-id="e589d-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="e589d-122">Tesztelje az alkalmazást annak ellenőrzéséhez, hogy nem működik-e natív módon.</span><span class="sxs-lookup"><span data-stu-id="e589d-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="e589d-123">Sok webhely kínál modern tartalmakat, amikor modern böngészőt észlel, és csak régi tartalmakat ajánl fel, amikor az Internet Explorert észleli.</span><span class="sxs-lookup"><span data-stu-id="e589d-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="e589d-124">Vegye fel az appot a vállalati webhelylistára, ha nem tudja tesztelni.</span><span class="sxs-lookup"><span data-stu-id="e589d-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="e589d-125">Gyakorlati megoldásként csoportosítsa az appot magában foglaló összes webhelyet.</span><span class="sxs-lookup"><span data-stu-id="e589d-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="e589d-126">Ily módon az appok frissítésekkor egyszerűbben távolíthatja el a teljes webhelyet az Internet Explorer módból, és elkezdheti használni az app modern böngészőjét.</span><span class="sxs-lookup"><span data-stu-id="e589d-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="e589d-127">Ha végzett a webhelyfeltárással, és elemezte az adatokat, készen áll a csatornastratégia elemzésére.</span><span class="sxs-lookup"><span data-stu-id="e589d-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

