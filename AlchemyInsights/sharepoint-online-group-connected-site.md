---
title: Csoport hozzáadása egy SharePoint-webhely
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507849"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="420b8-102">Kérdések létrehozása vagy a csoport kapcsolat a SharePoint Online webhelyek</span><span class="sxs-lookup"><span data-stu-id="420b8-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="420b8-103">Van néhány általános problémát észlelt létrehozása, vagy hozza létre újra a csoport webhely kapcsolat.</span><span class="sxs-lookup"><span data-stu-id="420b8-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="420b8-104">Ha törölt egy csoport és a kapcsolódó webhely, és létrehoz egy másik webhely ugyanazt az URL-címmel, szüksége lesz a végleges eltávolítása az előző webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="420b8-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="420b8-105">[Sao felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése</span><span class="sxs-lookup"><span data-stu-id="420b8-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="420b8-106">További információ a Bevezetés a powershell lásd: [Bevezetés a SharePoint Online felügyeleti rendszerhéj](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="420b8-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="420b8-107">Távolítsa el a webhely törölt helyek az [Eltávolítás-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="420b8-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="420b8-108">Ha készítünk egy csoport kapcsolattal rendelkező hely, és már létezik egy másik csoportot ugyanazzal az aliasnévvel rendelkező figyelmeztetést kap, ellenőrizze az [Office 365 felügyeleti központból a](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)meglévő csoportjait.</span><span class="sxs-lookup"><span data-stu-id="420b8-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="420b8-109">A probléma megoldásához, törli a meglévő csoportot, ha már nincs szüksége, vagy hozzon létre egy másikat a webhely kap.</span><span class="sxs-lookup"><span data-stu-id="420b8-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="420b8-110">Különböző módon lehet létrehozni és modern csoportok használata a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="420b8-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="420b8-111">Az Office 365 csoport meglévő webhelyekhez csatlakozhat.</span><span class="sxs-lookup"><span data-stu-id="420b8-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="420b8-112">További információért lásd: [Csatlakozás az Office 365 csoport segítségével a SharePoint felhasználói ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="420b8-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="420b8-113">Az Office 365 csoport kapcsolattal rendelkező hely létrehozásához szüksége lesz a csoportwebhely létrehozása.</span><span class="sxs-lookup"><span data-stu-id="420b8-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="420b8-114">További információért lásd: [Create a SharePoint csoportwebhelyet](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="420b8-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

