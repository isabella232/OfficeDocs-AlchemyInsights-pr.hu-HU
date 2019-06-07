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
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758733"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="eea6d-102">A SharePoint Online kapcsolattal rendelkező hely csoport létrehozása</span><span class="sxs-lookup"><span data-stu-id="eea6d-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="eea6d-103">Van néhány általános problémát észlelt létrehozása, vagy hozza létre újra a csoport webhely kapcsolat.</span><span class="sxs-lookup"><span data-stu-id="eea6d-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="eea6d-104">Ha törölt egy csoport és a kapcsolódó webhely, és létrehoz egy másik webhely ugyanazt az URL-címmel, szüksége lesz a végleges eltávolítása az előző webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="eea6d-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="eea6d-105">[Sao felügyeleti rendszerhéj](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) letöltése</span><span class="sxs-lookup"><span data-stu-id="eea6d-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="eea6d-106">További információ a Bevezetés a powershell lásd: [Bevezetés a SharePoint Online felügyeleti rendszerhéj](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="eea6d-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="eea6d-107">Távolítsa el a webhely törölt helyek az [Eltávolítás-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="eea6d-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="eea6d-108">Ha készítünk egy csoport kapcsolattal rendelkező hely, és már létezik egy másik csoportot ugyanazzal az aliasnévvel rendelkező figyelmeztetést kap, ellenőrizze az [Office 365 felügyeleti központból a](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)meglévő csoportjait.</span><span class="sxs-lookup"><span data-stu-id="eea6d-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="eea6d-109">A probléma megoldásához, törli a meglévő csoportot, ha már nincs szüksége, vagy hozzon létre egy másikat a webhely kap.</span><span class="sxs-lookup"><span data-stu-id="eea6d-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="eea6d-110">Különböző módon lehet létrehozni és modern csoportok használata a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eea6d-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="eea6d-111">Az Office 365 csoport meglévő webhelyekhez csatlakozhat.</span><span class="sxs-lookup"><span data-stu-id="eea6d-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="eea6d-112">További információért lásd: [Csatlakozás az Office 365 csoport segítségével a SharePoint felhasználói ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="eea6d-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="eea6d-113">Az Office 365 csoport kapcsolattal rendelkező hely létrehozásához szüksége lesz a csoportwebhely létrehozása.</span><span class="sxs-lookup"><span data-stu-id="eea6d-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="eea6d-114">További információért lásd: [Create a SharePoint csoportwebhelyet](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="eea6d-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

