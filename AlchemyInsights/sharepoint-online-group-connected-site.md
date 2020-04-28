---
title: Csoport hozzáadása SharePoint-webhelyhez
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
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912968"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="dabde-102">Problémák a csoportos csatlakoztatott webhely SharePoint-ban történő létrehozásakor</span><span class="sxs-lookup"><span data-stu-id="dabde-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="dabde-103">A csoporthoz csatlakoztatott hely létrehozása vagy újbóli létrehozása során gyakran előforduló gyakori problémák.</span><span class="sxs-lookup"><span data-stu-id="dabde-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="dabde-104">Ha törölt egy csoportot és annak csatlakoztatott webhelyét, és egy másik webhelyet szeretne létrehozni ugyanazzal az URL-címmel, véglegesen el kell távolítania az előző webhelyet.</span><span class="sxs-lookup"><span data-stu-id="dabde-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="dabde-105">[SPO-felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése</span><span class="sxs-lookup"><span data-stu-id="dabde-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="dabde-106">A PowerShell kezelésének megkezdéséről a [SharePoint Online Felügyeleti rendszerhéj – első lépések](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)ebben az esetben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="dabde-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="dabde-107">Távolítsa el a helyet a törölt helyekről az [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="dabde-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="dabde-108">A Powershell szükséges a csoportwebhelyek végleges törléséhez.</span><span class="sxs-lookup"><span data-stu-id="dabde-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="dabde-109">Ha csoporthoz csatlakoztatott webhelyet hoz létre, és figyelmeztetést kap: **Már létezik egy másik, azonos aliassal rendelkező csoport,** ellenőrizze a meglévő csoportokat a [Microsoft 365 Felügyeleti központban.](https://admin.microsoft.com/AdminPortal/Home#/groups)</span><span class="sxs-lookup"><span data-stu-id="dabde-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="dabde-110">A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozzon létre egy másik aliast hozzárendelt webhelyet.</span><span class="sxs-lookup"><span data-stu-id="dabde-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="dabde-111">A SharePoint segítségével különböző módokon hozhat létre és használhat modern csoportokat.</span><span class="sxs-lookup"><span data-stu-id="dabde-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="dabde-112">Meglévő helyeket microsoft 365-csoporthoz kapcsolhat.</span><span class="sxs-lookup"><span data-stu-id="dabde-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="dabde-113">További információt a [Microsoft 365-csoport csatlakoztatása a SharePoint felhasználói felületén című témakörben](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)talál.</span><span class="sxs-lookup"><span data-stu-id="dabde-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="dabde-114">Microsoft 365 csoporthoz csatlakoztatott webhely létrehozásához [csoportwebhelyet kell létrehoznia.](https://admin.microsoft.com/sharepoint)</span><span class="sxs-lookup"><span data-stu-id="dabde-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
