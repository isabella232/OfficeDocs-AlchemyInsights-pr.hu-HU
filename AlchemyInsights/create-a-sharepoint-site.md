---
title: A SharePoint-webhely létrehozása
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515809"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="2771c-102">A SharePoint-webhely létrehozása</span><span class="sxs-lookup"><span data-stu-id="2771c-102">Create a SharePoint site</span></span>

<span data-ttu-id="2771c-103">További információt a SharePoint-webhely létrehozása a következő látható:</span><span class="sxs-lookup"><span data-stu-id="2771c-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="2771c-104">[Az új SharePoint-felügyeleti központ a helyek kezelése](https://docs.microsoft.com/sharepoint/manage-site-creation): tudnivalók a webhely létrehozási beállítások, többek között a klasszikus vagy egy csapatok helyen, amely nem tartalmazza az Office 365 csoport létrehozása.</span><span class="sxs-lookup"><span data-stu-id="2771c-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="2771c-105">[Létrehozása a SharePoint csoportwebhelyet](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Útmutató a csoportwebhely létrehozása.</span><span class="sxs-lookup"><span data-stu-id="2771c-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="2771c-106">[A SharePoint Online kommunikáció hely létrehozása](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Útmutató kommunikációs webhelyet hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="2771c-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="2771c-107">[Az új SharePoint-felügyeleti központ a helyek kezelése](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Útmutató a klasszikus vagy egy csoport helyen, amely nem tartalmazza az Office 365 csoport létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="2771c-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Tippek]
> - <span data-ttu-id="2771c-109">A webhely nem hozható létre azonos egy meglévő webhely URL-címét.</span><span class="sxs-lookup"><span data-stu-id="2771c-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="2771c-110">Ha törli egy webhely, és újra használni az URL-cím kívánó, lehetőség a törölt hely továbbra is a **Törölt helyek**alatt.</span><span class="sxs-lookup"><span data-stu-id="2771c-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="2771c-111">Kezelheti a helyek Lásd, [törölheti a webhelyet](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)törli.</span><span class="sxs-lookup"><span data-stu-id="2771c-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="2771c-112">A Powershell webhely teljes eltávolításához az [Eltávolítás-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) parancsmag példa látható</span><span class="sxs-lookup"><span data-stu-id="2771c-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="2771c-113">Egyes felhasználók nem lehet webhelyet hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="2771c-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="2771c-114">Lásd: [Manage webhely létrehozása a SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="2771c-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="2771c-115">Akkor lehet a webhely **létrehozása** a vártnál több a rögzített jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="2771c-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="2771c-116">24 óránál hosszabb idő telt el azóta, először látta a probléma, ha jelentkezzen egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="2771c-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2771c-117">Sok esetben azt már dolgozik a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="2771c-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2771c-118">Adja meg a megoldás végrehajtásához legalább 24 órán keresztül.</span><span class="sxs-lookup"><span data-stu-id="2771c-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="2771c-119">Ha létre kell hoznia egy új csoportwebhely, amely nem tartalmazza az Office 365 csoport</span><span class="sxs-lookup"><span data-stu-id="2771c-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


