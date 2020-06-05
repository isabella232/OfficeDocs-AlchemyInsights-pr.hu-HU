---
title: 2609-retenció-vagy-elektronikus felfedezés-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 4d2b36fb78390f32d68f1cdd11ca1af8013424a2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576886"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="ffdd8-102">Nem lehet törölni az elemeket a SharePoint Online-ban vagy a OneDrive Vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="ffdd8-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="ffdd8-103">Előfordulhat, hogy Ön vagy a felhasználók nem tudják törölni a SharePoint Online vagy a OneDrive Vállalati verzió elemeit, mert adatmegőrzési házirend, adatmegőrzési címke vagy elektronikus adatfeltárási visszatartás van alkalmazva a OneDrive-webhelyek sharePoint-webhelyére vagy egy adott elemre.</span><span class="sxs-lookup"><span data-stu-id="ffdd8-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="ffdd8-104">Ez magában foglalja a dokumentum, a dokumentumverzió, a mappa, a dokumentumtár, a lista, az alkalmazás, a webhely vagy a webhelycsoport törlését.</span><span class="sxs-lookup"><span data-stu-id="ffdd8-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="ffdd8-105">Az ilyen esetek valamelyikében lévő elemek törléséhez el kell távolítani az adatmegőrzési szabályt, az adatmegőrzési címkét vagy az elektronikus adatfeltárási visszatartást (vagy egy helyet ki kell zárni az adatmegőrzési szabályból).</span><span class="sxs-lookup"><span data-stu-id="ffdd8-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="ffdd8-106">Le kell tiltania vagy ki kell zárnia a problémát okozó megfelelő visszatartást.</span><span class="sxs-lookup"><span data-stu-id="ffdd8-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="ffdd8-107">Az adatmegőrzési szabály vagy a visszatartás eltávolítása után akár 24 órát is igénybe vehet, amíg a módosítás érvénybe lép.</span><span class="sxs-lookup"><span data-stu-id="ffdd8-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="ffdd8-108">A SharePoint-webhelyekre és OneDrive-fiókokra alkalmazható különböző megőrzési és visszatartási funkciókról az alábbi témakörökben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="ffdd8-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="ffdd8-109">Adatmegőrzési házirendek – áttekintés</span><span class="sxs-lookup"><span data-stu-id="ffdd8-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="ffdd8-110">Megőrzési címkék áttekintése</span><span class="sxs-lookup"><span data-stu-id="ffdd8-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="ffdd8-111">Visszatartja kezelése a speciális elektronikus adatfeltárásban</span><span class="sxs-lookup"><span data-stu-id="ffdd8-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="ffdd8-112">elektronikus adatfeltárás visszatartja</span><span class="sxs-lookup"><span data-stu-id="ffdd8-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="ffdd8-113">Örökölt webhely-lezárási és törlési házirendek</span><span class="sxs-lookup"><span data-stu-id="ffdd8-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)