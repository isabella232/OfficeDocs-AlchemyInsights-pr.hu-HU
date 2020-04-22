---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive-on
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692767"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="87336-102">Hozzáférés korlátozása a SharePointban vagy a OneDrive-on</span><span class="sxs-lookup"><span data-stu-id="87336-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="87336-103">A SharePoint Online-szolgáltatásokhoz/OneDrive-szolgáltatásokhoz való hozzáférés számos módon korlátozhatja a hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="87336-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="87336-104">Ezeket a különböző hozzáférés-korlátozási módszereket az alábbiakban ismertetjük.</span><span class="sxs-lookup"><span data-stu-id="87336-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="87336-105">**Engedélykorlátozás**</span><span class="sxs-lookup"><span data-stu-id="87336-105">**Permission Restriction**</span></span>

<span data-ttu-id="87336-106">A SharePoint Online-ban és a OneDrive Vállalati verzióban úgy korlátozzuk a hozzáférést az olyan elemekhez, mint a webhelyek, fájlok és mappák, ha csak azoknak a csoportoknak/személyeknek biztosítunk hozzáférést, akiknek hozzáféréssel kell rendelkezniük.</span><span class="sxs-lookup"><span data-stu-id="87336-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="87336-107">SharePoint-lista vagy tár engedélyeinek testreszabása</span><span class="sxs-lookup"><span data-stu-id="87336-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="87336-108">SharePoint-webhely engedélyeinek testreszabása</span><span class="sxs-lookup"><span data-stu-id="87336-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="87336-109">Almappa engedélyeinek módosítása</span><span class="sxs-lookup"><span data-stu-id="87336-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="87336-110">Nem kezelt eszközök hozzáférésének kezelése</span><span class="sxs-lookup"><span data-stu-id="87336-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="87336-111">SharePoint- vagy globális rendszergazdaként letilthatja vagy korlátozhatja a SharePoint- és OneDrive-tartalmakhoz való hozzáférést nem felügyelt eszközökről (amelyek nem hibrid AD-hez csatlakoztak vagy nem kompatibilisek az Intune-ban).</span><span class="sxs-lookup"><span data-stu-id="87336-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="87336-112">**Hálózati hely korlátozása**</span><span class="sxs-lookup"><span data-stu-id="87336-112">**Network Location Restriction**</span></span>

<span data-ttu-id="87336-113">Informatikai rendszergazdaként szabályozhatja a SharePoint- és OneDrive-erőforrásokhoz való hozzáférést a megvetett hálózati helyek alapján.</span><span class="sxs-lookup"><span data-stu-id="87336-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="87336-114">Ezt helyalapú házirendnek is nevezik.</span><span class="sxs-lookup"><span data-stu-id="87336-114">This is also known as location-based policy.</span></span> <span data-ttu-id="87336-115">További információt a [SharePoint Online-adatokhoz való hozzáférés szabályozása a hálózati hely alapján](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="87336-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="87336-116">**Webhelyzárolás korlátozása**</span><span class="sxs-lookup"><span data-stu-id="87336-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="87336-117">A SharePoint Online-on belül zárolhat egy webhelycsoportot, így senki sem férhet hozzá.</span><span class="sxs-lookup"><span data-stu-id="87336-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="87336-118">Ez a PowerShell és a [SharePoint Online felügyeleti rendszerhéj](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) on keresztül a [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState tulajdonság használatával van beállítva.</span><span class="sxs-lookup"><span data-stu-id="87336-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="87336-119">**A felhasználók webhelyek vagy alwebhelyek létrehozásának korlátozása**</span><span class="sxs-lookup"><span data-stu-id="87336-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="87336-120">SharePoint-rendszergazdaként vagy globális rendszergazdaként lehetővé teheti a felhasználók számára, hogy saját SharePoint-webhelyeket hozzanak létre és felügyeljenek, meghatározzák, hogy milyen webhelyeket hozhatnak létre, és megadhatja a webhelyek helyét.</span><span class="sxs-lookup"><span data-stu-id="87336-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="87336-121">További információt a [Webhelylétrehozásának kezelése a SharePoint Online-ban című témakörben talál.](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="87336-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

