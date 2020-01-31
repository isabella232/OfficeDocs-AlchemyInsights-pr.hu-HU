---
title: 2609-megtartás-vagy-ediscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 3e60f0fc53cd78c9cc816a658a9df05e9075e26e
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571316"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="a147a-102">Nem lehet törölni az elemeket a SharePoint Online-ban vagy a OneDrive Vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="a147a-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="a147a-103">Előfordulhat, hogy Ön vagy a felhasználók nem tudják törölni a SharePoint Online vagy a OneDrive Vállalati verzió elemeit, mert adatmegőrzési házirend, adatmegőrzési címke vagy elektronikus adatfeltárási adatmegőrzési adatszolgáltatás a OneDrive-webhely SharePointjára vagy egy adott elemre vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="a147a-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="a147a-104">Ez magában foglalja a dokumentum, a dokumentumverzió, a mappa, a dokumentumtár, a lista, az alkalmazás, a webhely vagy a webhelycsoport törlésének nem módját.</span><span class="sxs-lookup"><span data-stu-id="a147a-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="a147a-105">Az ilyen esetek valamelyikében lévő elemek törléséhez el kell távolítani az adatmegőrzési szabályt, az adatmegőrzési címkét vagy az elektronikus adatfeltárási várakoztatási adatmegőrzési szabályt (vagy egy webhelyet ki kell zárni az adatmegőrzési szabályból).</span><span class="sxs-lookup"><span data-stu-id="a147a-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="a147a-106">Le kell tiltania vagy ki kell zárnia a problémát okozó megfelelő tartást.</span><span class="sxs-lookup"><span data-stu-id="a147a-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="a147a-107">Az adatmegőrzési szabályzat vagy a letartás eltávolítása után akár 24 órát is igénybe vehet a módosítás érvénybe léptetése.</span><span class="sxs-lookup"><span data-stu-id="a147a-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="a147a-108">A SharePoint-webhelyekre és OneDrive-fiókokra alkalmazható különböző megőrzési és adatmegőrzési funkciókról az alábbi témakörök ben olvashat.</span><span class="sxs-lookup"><span data-stu-id="a147a-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="a147a-109">Adatmegőrzési házirendek áttekintése</span><span class="sxs-lookup"><span data-stu-id="a147a-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="a147a-110">A megőrzési címkék áttekintése</span><span class="sxs-lookup"><span data-stu-id="a147a-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="a147a-111">A speciális elektronikus adatfeltárás iratitási tartamának kezelése</span><span class="sxs-lookup"><span data-stu-id="a147a-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="a147a-112">az elektronikus adatfeltárás tart</span><span class="sxs-lookup"><span data-stu-id="a147a-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="a147a-113">Örökölt webhelylezárási és törlési házirendek</span><span class="sxs-lookup"><span data-stu-id="a147a-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)