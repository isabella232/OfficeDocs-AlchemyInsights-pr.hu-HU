---
title: A SharePoint Online keresés séma kezelése
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502809"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="f1b63-102">A SharePoint Online keresés séma kezelése</span><span class="sxs-lookup"><span data-stu-id="f1b63-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="f1b63-103">A search séma meghatározza, milyen felhasználók kereshetnek, hogyan felhasználók kereshetnek, és hogyan lehet megjeleníteni az eredményeket a keresési webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="f1b63-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="f1b63-104">Lásd: további információt [a SharePoint online keresés séma kezelése](https://docs.microsoft.com/sharepoint/manage-search-schema) módjáról:</span><span class="sxs-lookup"><span data-stu-id="f1b63-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="f1b63-105">A search séma módosítása.</span><span class="sxs-lookup"><span data-stu-id="f1b63-105">Change the search schema.</span></span>
- <span data-ttu-id="f1b63-106">A felügyelt tulajdonságok létrehozása.</span><span class="sxs-lookup"><span data-stu-id="f1b63-106">Create managed properties.</span></span>
- <span data-ttu-id="f1b63-107">Bejárt adatleképezést bejárt tulajdonságok felügyelt tulajdonságokra.</span><span class="sxs-lookup"><span data-stu-id="f1b63-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="f1b63-108">Megjegyzés: a Search séma kezelése esetében a következő:</span><span class="sxs-lookup"><span data-stu-id="f1b63-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="f1b63-109">Arról **az alkalmazás fel van függesztve** , a séma módosítása, ha figyelmeztetést kap, ha ez csak ideiglenes karbantartási szolgáltatás nem fordul elő.</span><span class="sxs-lookup"><span data-stu-id="f1b63-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="f1b63-110">Ha több mint 24 óra estek át, és továbbra is észleli a figyelmeztető üzenet, jelentkezzen be támogatási eset.</span><span class="sxs-lookup"><span data-stu-id="f1b63-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="f1b63-111">Felügyelt tulajdonságok módosítása, vagy újakat vehet fel, ha a változások lépnek érvénybe, amikor a tartalom már bejárását.</span><span class="sxs-lookup"><span data-stu-id="f1b63-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="f1b63-112">A SharePoint Online bejárás történik alapján automatikusan a megadott bejárási ütemezés.</span><span class="sxs-lookup"><span data-stu-id="f1b63-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="f1b63-113">Győződjön meg arról, hogy a módosítások bejárását végzi, hogy kifejezetten [a lista vagy tár újból indexelő kérés](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) is</span><span class="sxs-lookup"><span data-stu-id="f1b63-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="f1b63-114">A Search séma teljes körű áttekintést talál [Search séma bevezetéséről](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="f1b63-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


