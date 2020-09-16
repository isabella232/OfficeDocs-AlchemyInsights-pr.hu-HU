---
title: 2609-adatmegőrzési vagy eDiscovery
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727893"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="32747-102">Nem lehet elemeket törölni a SharePoint Online-ban vagy a OneDrive vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="32747-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="32747-103">Előfordulhat, hogy Ön vagy a felhasználók nem tudják törölni az elemeket a SharePoint Online-ban vagy a OneDrive vállalati verzióban, mert az adatmegőrzési házirend, a adatmegőrzési címke vagy a eDiscovery mentességet alkalmazza a OneDrive-webhelyre vagy egy adott elemre.</span><span class="sxs-lookup"><span data-stu-id="32747-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="32747-104">Ez a funkció a dokumentumok, a dokumentumok, a mappák, a dokumentumtárak, a listák, az alkalmazások, a webhelyek és a webhelycsoport törlésére is használható.</span><span class="sxs-lookup"><span data-stu-id="32747-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="32747-105">Ha a fenti esetek egyikében törölni szeretné az elemeket, el kell távolítania az adatmegőrzési házirendet, a adatmegőrzési címkét vagy a eDiscovery mentességet (vagy egy webhelyet ki kell zárni egy adatmegőrzési házirendből).</span><span class="sxs-lookup"><span data-stu-id="32747-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="32747-106">A problémát okozó mentességet le kell tiltania vagy ki kell zárnia.</span><span class="sxs-lookup"><span data-stu-id="32747-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="32747-107">Az adatmegőrzési házirend vagy a mentesség eltávolítása után akár 24 óra is eltelhet, amíg a módosítás érvénybe lép.</span><span class="sxs-lookup"><span data-stu-id="32747-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="32747-108">A SharePoint-webhelyeken és a OneDrive-fiókokban alkalmazható különböző adatmegőrzési és mentességi funkciókról az alábbi témakörökben tájékozódhat.</span><span class="sxs-lookup"><span data-stu-id="32747-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="32747-109">Adatmegőrzési házirendek – áttekintés</span><span class="sxs-lookup"><span data-stu-id="32747-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="32747-110">Az adatmegőrzési címkék áttekintése</span><span class="sxs-lookup"><span data-stu-id="32747-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="32747-111">A mentességek kezelése a speciális eDiscovery</span><span class="sxs-lookup"><span data-stu-id="32747-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="32747-112">eDiscovery tart</span><span class="sxs-lookup"><span data-stu-id="32747-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="32747-113">Korábbi webhely bezárása és törlési házirendek</span><span class="sxs-lookup"><span data-stu-id="32747-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)