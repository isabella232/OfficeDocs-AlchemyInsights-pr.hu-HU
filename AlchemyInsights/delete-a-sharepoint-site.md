---
title: A SharePoint-webhely törlése
ms.author: kirks
author: Techwriter40
ms.date: 1/24/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c060815d-1d3f-4a13-81c2-0377bbeda202
ms.openlocfilehash: f6ee16a20f2280ba4d8d28ab3fdb4672cd9963b5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927578"
---
# <a name="delete-a-sharepoint-site"></a><span data-ttu-id="29dfc-102">A SharePoint-webhely törlése</span><span class="sxs-lookup"><span data-stu-id="29dfc-102">Delete a SharePoint site</span></span>
 <span data-ttu-id="29dfc-103">**Az új SharePoint-felügyeleti központ helyek törlése**</span><span class="sxs-lookup"><span data-stu-id="29dfc-103">**Delete sites from the new SharePoint admin center**</span></span>
  
<span data-ttu-id="29dfc-p101">Az aktív webhely törlése, Ugrás az aktuális SharePoint admin center, kattintson a "Próbálja ki most" a jobb felső részén. Jelölje be az **aktív helyek**, válassza ki a webhelyet, és válassza a **Törlés**. [Nézet és a visszaállítás törli az új SharePoint-felügyeleti központ webhelyet](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)jelölje be a **Törölt helyek**. További információért lásd: [az új SharePoint-felügyeleti központ a helyek kezelése](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).</span><span class="sxs-lookup"><span data-stu-id="29dfc-p101">To delete an active site, go to the current SharePoint admin center, click "Try it now" in the upper right. Select **Active sites**, select the site, and then select **Delete**. To [view and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center), select **Deleted sites**. For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).</span></span>
  
<span data-ttu-id="29dfc-p102">**Fontos:** Ha a webhely adatmegőrzési része, nem lehet törölhető, amíg a webhely eltűnik a [biztonsági &amp; megfelelési Admin Center](https://protection.office.com/?rfr=AdminCenter#/homepage). További információért lásd: [Adatmegőrzési szabályok áttekintése](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites) .</span><span class="sxs-lookup"><span data-stu-id="29dfc-p102">**Important:** If the site is part of a retention policy, you may not be able to delete it until the site is removed from the [Security &amp; Compliance Admin Center](https://protection.office.com/?rfr=AdminCenter#/homepage). See [Overview of Retention Policies](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites) for more info.</span></span> 
  
<span data-ttu-id="29dfc-110">Tippek:</span><span class="sxs-lookup"><span data-stu-id="29dfc-110">Tips:</span></span>
- <span data-ttu-id="29dfc-p103">Globális rendszergazdák és a SharePoint Rendszergazdák most már törölheti az **Office 365 csoporthoz**tartozó helyek. Ezzel törli a csoport és összes forrásai, beleértve az Outlook postafiók és a naptár és a csapatok csatornák. További információért lásd: a [SharePoint-webhely törlése](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="29dfc-p103">Global admins and SharePoint admins can now delete sites that belong to an **Office 365 Group**. This will delete the group and all its resources, including the Outlook mailbox and calendar, and any Teams channels. For more info, see [Delete a SharePoint site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span></span>
- <span data-ttu-id="29dfc-p104">Visszaállíthatja a törölt helyek 93 napra. Fontos megjegyezni, hogy a törölt csoport 30 napon belül kell visszaállítani. További információért lásd a [nézet és a visszaállítás törli a webhelyek](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center).</span><span class="sxs-lookup"><span data-stu-id="29dfc-p104">You can recover deleted sites for 93 days. Note that deleted groups must be restored within 30 days. For more info, see [View and restore deleted sites](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center).</span></span>
- <span data-ttu-id="29dfc-117">A Powershell webhely teljes eltávolításához az [Eltávolítás-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) parancsmag példa látható</span><span class="sxs-lookup"><span data-stu-id="29dfc-117">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) cmdlet example.</span></span> 
  

