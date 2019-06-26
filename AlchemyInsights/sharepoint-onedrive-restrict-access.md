---
title: Korlátozza a hozzáférést a SharePoint- vagy OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223714"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="162b8-102">Korlátozza a hozzáférést a SharePoint- vagy OneDrive</span><span class="sxs-lookup"><span data-stu-id="162b8-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="162b8-103">Számos módon való hozzáférés korlátozása a SharePoint Online/OneDrive szolgáltatások.</span><span class="sxs-lookup"><span data-stu-id="162b8-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="162b8-104">E különböző hozzáférési korlátozás módszerek az alábbiakban vázolt.</span><span class="sxs-lookup"><span data-stu-id="162b8-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="162b8-105">**Engedélyek korlátozása**</span><span class="sxs-lookup"><span data-stu-id="162b8-105">**Permission Restriction**</span></span>

<span data-ttu-id="162b8-106">A SharePoint Online és az üzleti OneDrive azt korlátozza a hozzáférést elemekhez, például a webhelyek, fájlok és mappák csak a csoportok/személyek rendelkezzenek hozzáféréssel való hozzáférés biztosítása által.</span><span class="sxs-lookup"><span data-stu-id="162b8-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="162b8-107">SharePoint-lista vagy tár engedélyeinek testreszabása</span><span class="sxs-lookup"><span data-stu-id="162b8-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="162b8-108">A SharePoint webhely engedélyeinek testreszabására</span><span class="sxs-lookup"><span data-stu-id="162b8-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="162b8-109">Almappa engedélyeinek módosítása</span><span class="sxs-lookup"><span data-stu-id="162b8-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="162b8-110">Nem kezelt eszközök hozzáférésének kezelése</span><span class="sxs-lookup"><span data-stu-id="162b8-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="162b8-111">SharePoint vagy az Office 365 globális rendszergazda zárolhatja vagy korlátozza a hozzáférést a SharePoint-és OneDrive a nem kezelt eszközök (a hibrid illesztett vagy kompatibilis az Intune AD).</span><span class="sxs-lookup"><span data-stu-id="162b8-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="162b8-112">**Hálózati hely korlátozás**</span><span class="sxs-lookup"><span data-stu-id="162b8-112">**Network Location Restriction**</span></span>

<span data-ttu-id="162b8-113">INFORMATIKAI rendszergazdaként szabályozhatja a meghatározott hálózati helyeken megbízható alapuló SharePoint és OneDrive erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="162b8-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="162b8-114">Ez a hely alapú házirend néven is ismert.</span><span class="sxs-lookup"><span data-stu-id="162b8-114">This is also known as location-based policy.</span></span> <span data-ttu-id="162b8-115">További információt talál [a SharePoint Online és a OneDrive adatok hálózati hely alapján való hozzáférés szabályozása](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="162b8-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="162b8-116">**Webhelykorlátozás zárolása**</span><span class="sxs-lookup"><span data-stu-id="162b8-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="162b8-117">SharePoint Online belül, hogy a számítógép zárolásához a webhelycsoportot, így ne hozzáférése van.</span><span class="sxs-lookup"><span data-stu-id="162b8-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="162b8-118">A PowerShell és a [SharePoint Online felügyeleti rendszerhéj](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) segítségével a [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState tulajdonság értéke.</span><span class="sxs-lookup"><span data-stu-id="162b8-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="162b8-119">**Webhelyek és alwebhelyek létrehozását követően a felhasználók korlátozása**</span><span class="sxs-lookup"><span data-stu-id="162b8-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="162b8-120">A SharePoint felügyeleti vagy Office 365 globális felügyeleti lehetővé teszik a felhasználók létrehozása és a saját SharePoint-webhelyek felügyelete, meghatározza, milyen típusú webhelyeket hozhatnak létre, és a webhelyek elérési útja.</span><span class="sxs-lookup"><span data-stu-id="162b8-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="162b8-121">További információért lásd [kezelés webhely létrehozása a SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="162b8-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

