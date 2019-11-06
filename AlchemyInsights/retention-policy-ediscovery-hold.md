---
title: 2609-visszatartás-or-eDiscovery-Hold
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
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994070"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="c5073-102">Nem lehet törölni az elemeket a SharePoint Online szolgáltatásban vagy az OneDrive for Business alkalmazásban</span><span class="sxs-lookup"><span data-stu-id="c5073-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="c5073-103">Előfordulhat, hogy a felhasználó vagy a felhasználók nem törölhetnek elemeket a SharePoint Online szolgáltatásban vagy az OneDrive for Business alkalmazásban, mert az adatmegőrzési házirendet, az adatmegőrzési címkét vagy az eDiscovery visszatartást alkalmazza a SharePoint OneDrive webhelyre vagy egy adott elemre.</span><span class="sxs-lookup"><span data-stu-id="c5073-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="c5073-104">Ez azt is magában foglalja, hogy nem törölhető egy dokumentum, egy dokumentumverzió, egy mappa, egy dokumentumtár, egy lista, egy alkalmazás, egy webhely vagy egy webhelycsoport.</span><span class="sxs-lookup"><span data-stu-id="c5073-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="c5073-105">Néhány példa azokra a hibaüzenetekkel kapcsolatban, amelyeket akkor kapott, ha egy megőrzendő elemet próbál törölni:</span><span class="sxs-lookup"><span data-stu-id="c5073-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="c5073-106">"Ez a webhely nem törölhető, mert szerepel egy eDiscovery visszatartási vagy adatmegőrzési házirendben"</span><span class="sxs-lookup"><span data-stu-id="c5073-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="c5073-107">"A webhelynek van egy megfelelőségi házirendje, amely a törlés blokkolására van beállítva"</span><span class="sxs-lookup"><span data-stu-id="c5073-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="c5073-108">"A megfelelőségi házirend jelenleg blokkolja a webhely törlését"</span><span class="sxs-lookup"><span data-stu-id="c5073-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="c5073-109">"Ez a webhelycsoport nem törölhető, mert olyan webhelyeket tartalmaz, amelyek egy eDiscovery visszatartási vagy adatmegőrzési házirendben szerepelnek"</span><span class="sxs-lookup"><span data-stu-id="c5073-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="c5073-110">"Önnek van-hoz töröl minden a cikk ebben dosszié előtted töröl a dosszié"</span><span class="sxs-lookup"><span data-stu-id="c5073-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="c5073-111">"Az elem nem törölhető, mert tartási vagy adatmegőrzési szabályban van"</span><span class="sxs-lookup"><span data-stu-id="c5073-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="c5073-112">"Az elem nem törölhető a visszatartott idő alatt"</span><span class="sxs-lookup"><span data-stu-id="c5073-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="c5073-113">"Az erre az elemre alkalmazott címke megakadályozza a szerkesztését vagy törlését"</span><span class="sxs-lookup"><span data-stu-id="c5073-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="c5073-114">"A lista nem törölhető, amíg a visszatartott vagy az adatmegőrzési szabályok"</span><span class="sxs-lookup"><span data-stu-id="c5073-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="c5073-115">"A listát nem lehet törölni, ha zárolva van, vagy ha egy adatmegőrzési házirendet alkalmaz"</span><span class="sxs-lookup"><span data-stu-id="c5073-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="c5073-116">A fenti esetek egyikében törölt elemek törléséhez az adatmegőrzési házirendet, az adatmegőrzési címkét vagy az eDiscovery visszatartást el kell távolítani (vagy egy webhelyet ki kell zárni az adatmegőrzési szabályból).</span><span class="sxs-lookup"><span data-stu-id="c5073-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="c5073-117">Sírnod kell egyik megbénít vagy kizár viszonylagos ragaszkodik amit ' okozás ez kérdés.</span><span class="sxs-lookup"><span data-stu-id="c5073-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="c5073-118">Az adatmegőrzési vagy visszatartási házirend eltávolítását követően a módosítás érvénybe léptetéséhez akár 24 óráig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="c5073-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="c5073-119">A SharePoint-webhelyekre és az OneDrive-fiókokhoz alkalmazható különböző megőrzési és tartási szolgáltatásokkal kapcsolatos további tudnivalókért tanulmányozza az alábbi témakörök egyikét.</span><span class="sxs-lookup"><span data-stu-id="c5073-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="c5073-120">Az adatmegőrzési szabályok áttekintése</span><span class="sxs-lookup"><span data-stu-id="c5073-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="c5073-121">Az adatmegőrzési címkék áttekintése</span><span class="sxs-lookup"><span data-stu-id="c5073-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="c5073-122">Kezel tart-ban haladó eDiscovery</span><span class="sxs-lookup"><span data-stu-id="c5073-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="c5073-123">eDiscovery tartja</span><span class="sxs-lookup"><span data-stu-id="c5073-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="c5073-124">Örökölt webhely-bezárási és törlési házirendek</span><span class="sxs-lookup"><span data-stu-id="c5073-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
