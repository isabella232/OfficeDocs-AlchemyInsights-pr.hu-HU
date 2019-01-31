---
title: A SharePoint-webhely létrehozása
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 92bb7b5f0a684936db52f6be9e00c8dff3378bb5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657505"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="0d0cb-102">A SharePoint-webhely létrehozása</span><span class="sxs-lookup"><span data-stu-id="0d0cb-102">Create a SharePoint site</span></span>

<span data-ttu-id="0d0cb-p101">Webhely létrehozási beállítások [kezelése az új SharePoint-felügyeleti központ webhelyén](https://docs.microsoft.com/sharepoint/manage-site-creation ) talál. Jelölje be a [csoportwebhely](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (amely az Office 365 csoport jön létre) vagy egy [kommunikációs webhely](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)létrehozásához. [Klasszikus webhely](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)vagy egy új csoportwebhely, amely nem tartalmazza az Office 365 csoport létrehozásához kattintson az **egyéb beállítások**.</span><span class="sxs-lookup"><span data-stu-id="0d0cb-p101">See [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation ) for site creation options. Select to create a [team site](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (which will create an Office 365 group) or a [communication site](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). To create a [classic site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), or a new team site that doesn't include an Office 365 group, click **Other options**.</span></span> 
  
<span data-ttu-id="0d0cb-106">Tippek:</span><span class="sxs-lookup"><span data-stu-id="0d0cb-106">Tips:</span></span>
- <span data-ttu-id="0d0cb-107">*A webhely nem hozható létre azonos egy meglévő webhely URL-címét. Ha törli egy webhely, és újra használni az URL-cím kívánó, lehetőség a törölt hely továbbra is a **Törölt helyek**alatt. Kezelheti a helyek Lásd, [törölheti a webhelyet](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)törli. A Powershell webhely teljes eltávolításához az [Eltávolítás-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) parancsmag példa látható*</span><span class="sxs-lookup"><span data-stu-id="0d0cb-107">*You cannot create a site with the same URL of an existing site. If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**. To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.*</span></span>
- <span data-ttu-id="0d0cb-108">*Egyes felhasználók nem lehet webhelyet hozhat létre. Lásd: [Manage webhely létrehozása a SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span><span class="sxs-lookup"><span data-stu-id="0d0cb-108">*Some users may not be able to create a site. See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span></span>
- <span data-ttu-id="0d0cb-109">*Akkor lehet a webhely **létrehozása** a vártnál több a rögzített jelenik meg. 24 óránál hosszabb idő telt el azóta, először látta a probléma, ha jelentkezzen egy támogatási jegyet. Sok esetben azt már dolgozik a megoldáson. Adja meg a megoldás végrehajtásához legalább 24 órán keresztül.*</span><span class="sxs-lookup"><span data-stu-id="0d0cb-109">*It's possible the site appears stuck at **Creating** longer than expected. If more than 24 hours have passed since you first saw this issue, please log a support ticket. In many cases, we're already working on a solution. Please give us at least 24 hours to complete a solution.*</span></span>
