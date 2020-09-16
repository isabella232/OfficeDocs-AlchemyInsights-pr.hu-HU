---
title: Csoport felvétele SharePoint-webhelyre
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771206"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="88606-102">Problémák a csoporthoz csatlakoztatott SharePoint-webhelyek létrehozásakor</span><span class="sxs-lookup"><span data-stu-id="88606-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="88606-103">A csoporttal összekapcsolt webhelyek létrehozásakor vagy ismételt létrehozásakor előforduló gyakori problémák.</span><span class="sxs-lookup"><span data-stu-id="88606-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="88606-104">Ha törölt egy csoportot és a hozzá kapcsolódó webhelyet, és egy URL-lel másik webhelyet szeretne létrehozni, akkor véglegesen el kell távolítania az előző webhelyet.</span><span class="sxs-lookup"><span data-stu-id="88606-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="88606-105">A [Spongya felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése</span><span class="sxs-lookup"><span data-stu-id="88606-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="88606-106">A PowerShell használatáról további információt a [SharePoint Online felügyeleti rendszerhéj – első lépések](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="88606-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="88606-107">Távolítsa el a webhelyet a törölt webhelyekről a [Remove-SPODeletedSite PowerShell-](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="88606-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="88606-108">A csoport webhelyeinek végleges törléséhez PowerShell szükséges.</span><span class="sxs-lookup"><span data-stu-id="88606-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="88606-109">Ha egy csoporthoz kapcsolt webhelyet hoz létre, és figyelmeztetést jelenít meg: **egy másik, ugyanazzal az aliassal rendelkező csoport már létezik**, ellenőrizze a [Microsoft 365 felügyeleti központjának](https://admin.microsoft.com/AdminPortal/Home#/groups)meglévő csoportját.</span><span class="sxs-lookup"><span data-stu-id="88606-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="88606-110">A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozza létre azt a webhelyet, amelyhez másik alias van rendelve.</span><span class="sxs-lookup"><span data-stu-id="88606-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="88606-111">A modern csoportokat többféle módon hozhatja létre és használhatja a SharePointtal.</span><span class="sxs-lookup"><span data-stu-id="88606-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="88606-112">A meglévő webhelyeket összekapcsolhatja a Microsoft 365-csoporttal.</span><span class="sxs-lookup"><span data-stu-id="88606-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="88606-113">További információt a [Microsoft 365-csoport csatlakoztatása a SharePoint felhasználói felületéről](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="88606-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="88606-114">Ha létre szeretne hozni egy Microsoft 365-csoportot tartalmazó összekapcsolt webhelyet, létre kell hoznia egy [csoportwebhely](https://admin.microsoft.com/sharepoint)-webhelyet.</span><span class="sxs-lookup"><span data-stu-id="88606-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
