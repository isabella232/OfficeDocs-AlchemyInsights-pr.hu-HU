---
title: Csoport felvétele SharePoint-webhelyre
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770353"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="2e2a4-102">Problémák a csoporthoz kapcsolódó webhely SharePointban történő létrehozásakor</span><span class="sxs-lookup"><span data-stu-id="2e2a4-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="2e2a4-103">Néhány gyakori probléma, amely a csoporthoz kapcsolódó webhely létrehozásakor vagy újbóli létrehozásakor merült fel.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="2e2a4-104">Ha törölt egy csoportot és a kapcsolódó webhelyet, és egy másik webhelyet szeretne létrehozni ugyanazzal az URL-címmel, véglegesen el kell távolítania az előző webhelyet.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="2e2a4-105">[SPO felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése</span><span class="sxs-lookup"><span data-stu-id="2e2a4-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="2e2a4-106">A Powershell használatával kapcsolatos további tudnivalókért olvassa el [a SharePoint Online Felügyeleti rendszerhéj első](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)lépései .</span><span class="sxs-lookup"><span data-stu-id="2e2a4-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="2e2a4-107">Távolítsa el a webhelyet a törölt helyekről az [Eltávolítás-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell-parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="2e2a4-108">A Powershell szükséges a csoporthelyek végleges törléséhez.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="2e2a4-109">Ha csoporthoz kapcsolódó webhelyet hoz létre, és figyelmeztetést kap: **Már létezik egy másik, ugyanazzal az aliasnevű csoport,** ellenőrizze a meglévő csoportokat az [Office 365-ből a Felügyeleti központból.](https://admin.microsoft.com/AdminPortal/Home#/groups)</span><span class="sxs-lookup"><span data-stu-id="2e2a4-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="2e2a4-110">A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozzon létre egy másik aliast.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="2e2a4-111">A SharePoint tal különböző módokon hozhat létre és használhat modern csoportokat.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="2e2a4-112">A meglévő webhelyeket office 365-csoporthoz csatlakoztathatja.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="2e2a4-113">További információt [az Office 365-csoport csatlakoztatása a SharePoint felhasználói felületével](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="2e2a4-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="2e2a4-114">Office 365-csoporthoz kapcsolódó webhely létrehozásához létre kell hoznia egy [csoportwebhelyet.](https://admin.microsoft.com/sharepoint)</span><span class="sxs-lookup"><span data-stu-id="2e2a4-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
