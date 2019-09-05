---
title: Csoport hozzáadása SharePoint-webhelyhez
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750522"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="dddf7-102">Kapcsolódó webhelyek létrehozása vagy csoportosítása SharePoint Online szolgáltatásban – problémák</span><span class="sxs-lookup"><span data-stu-id="dddf7-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="dddf7-103">A csoporthoz kapcsolódó webhely létrehozásakor vagy ismételt létrehozásakor gyakran előforduló problémák merültek fel.</span><span class="sxs-lookup"><span data-stu-id="dddf7-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="dddf7-104">Ha törölt egy csoportot és a hozzá tartozó webhelyet, és egy másik webhelyet szeretne létrehozni ugyanazzal az URL-címmel, akkor véglegesen el kell távolítania az előző webhelyet.</span><span class="sxs-lookup"><span data-stu-id="dddf7-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="dddf7-105">Letöltés [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="dddf7-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="dddf7-106">További információ a PowerShell használatbaveléshez: [Ismerkedés a SharePoint Online Management Shell alkalmazással](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="dddf7-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="dddf7-107">Vegye ki a webhelyet a törölt webhelyekről a [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell parancsmaggal.</span><span class="sxs-lookup"><span data-stu-id="dddf7-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="dddf7-108">Ha csoportos kapcsolatban lévő webhelyet hoz létre, és figyelmeztetést kap, akkor már létezik egy másik, azonos aliasnévvel rendelkező csoport, és az Office 365 már meglévő csoportjait is ellenőrzi [a felügyeleti központból](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="dddf7-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="dddf7-109">A probléma megoldásához törölje a meglévő csoportot, ha már nincs rá szükség, vagy hozza létre a webhelyet egy másik aliasnévvel.</span><span class="sxs-lookup"><span data-stu-id="dddf7-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="dddf7-110">Különböző módokon hozhatók létre és használhatók a SharePoint rendszerben a modern csoportok.</span><span class="sxs-lookup"><span data-stu-id="dddf7-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="dddf7-111">A meglévő webhelyeket összekapcsolhatja egy Office 365-csoporttal.</span><span class="sxs-lookup"><span data-stu-id="dddf7-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="dddf7-112">További információ: [Office 365-csoport csatlakoztatása a SharePoint-felhasználó ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="dddf7-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="dddf7-113">Egy Office 365-csoporthoz kapcsolódó webhely létrehozásához létre kell hoznia egy csoportwebhelyet.</span><span class="sxs-lookup"><span data-stu-id="dddf7-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="dddf7-114">További információt a [csoportwebhely létrehozása a SharePoint szolgáltatásban](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="dddf7-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

