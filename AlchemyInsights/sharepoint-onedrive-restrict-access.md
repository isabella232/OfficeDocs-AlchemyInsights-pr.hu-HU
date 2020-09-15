---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700457"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="64bd3-102">Hozzáférés korlátozása a SharePointban vagy a OneDrive</span><span class="sxs-lookup"><span data-stu-id="64bd3-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="64bd3-103">A SharePoint Online-ban és az OneDrive-szolgáltatásokban többféleképpen korlátozhatja a hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="64bd3-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="64bd3-104">Ezek a különféle hozzáférési korlátozási módszerek alább láthatók.</span><span class="sxs-lookup"><span data-stu-id="64bd3-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="64bd3-105">**Jogosultság korlátozás**</span><span class="sxs-lookup"><span data-stu-id="64bd3-105">**Permission Restriction**</span></span>

<span data-ttu-id="64bd3-106">A SharePoint Online-ban és a OneDrive vállalati verzióban csak a webhelyek, a fájlok és a mappák hozzáférését korlátozzuk, ha hozzáférést szeretne adni azokhoz a csoportokhoz/egyénekhez, akiknek hozzáféréssel kell rendelkezniük.</span><span class="sxs-lookup"><span data-stu-id="64bd3-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="64bd3-107">SharePoint-lista vagy-tár engedélyeinek testreszabása</span><span class="sxs-lookup"><span data-stu-id="64bd3-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="64bd3-108">A SharePoint-webhely engedélyeinek testreszabása</span><span class="sxs-lookup"><span data-stu-id="64bd3-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="64bd3-109">Almappa engedélyeinek módosítása</span><span class="sxs-lookup"><span data-stu-id="64bd3-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="64bd3-110">Nem kezelt eszközök hozzáférésének kezelése</span><span class="sxs-lookup"><span data-stu-id="64bd3-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="64bd3-111">SharePoint-vagy globális rendszergazdaként letilthatja vagy korlátozhatja a SharePoint-és OneDrive-tartalmakat nem felügyelt eszközökről</span><span class="sxs-lookup"><span data-stu-id="64bd3-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="64bd3-112">**Hálózati hely korlátozás**</span><span class="sxs-lookup"><span data-stu-id="64bd3-112">**Network Location Restriction**</span></span>

<span data-ttu-id="64bd3-113">IT-rendszergazdaként a SharePoint-és OneDrive-erőforrásokhoz való hozzáférést a megbízhatóként megadott hálózati helyek alapján szabályozhatja.</span><span class="sxs-lookup"><span data-stu-id="64bd3-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="64bd3-114">Ez más néven hely-alapú házirend.</span><span class="sxs-lookup"><span data-stu-id="64bd3-114">This is also known as location-based policy.</span></span> <span data-ttu-id="64bd3-115">További információért olvassa el [a SharePoint Online és a OneDrive-adatok elérésének szabályozása hálózati hely alapján](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) című témakört.</span><span class="sxs-lookup"><span data-stu-id="64bd3-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="64bd3-116">**Webhely zárolásának korlátozása**</span><span class="sxs-lookup"><span data-stu-id="64bd3-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="64bd3-117">A SharePoint Online-ban lehetősége van egy webhelycsoport zárolására, így senki sem férhet hozzá.</span><span class="sxs-lookup"><span data-stu-id="64bd3-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="64bd3-118">Ez a beállítás a PowerShellen keresztül és a [SharePoint Online felügyeleti rendszerhéjon](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) keresztül érhető el a [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate tulajdonság használatával.</span><span class="sxs-lookup"><span data-stu-id="64bd3-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="64bd3-119">**Webhelyek és alwebhelyek létrehozásának korlátozása a felhasználóknak**</span><span class="sxs-lookup"><span data-stu-id="64bd3-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="64bd3-120">SharePoint-rendszergazdaként vagy globális rendszergazdává teheti a felhasználókat, hogy saját SharePoint-webhelyeket hozzanak létre és felügyelnek, meghatározhatja, hogy milyen típusú webhelyeket hozhat létre, és adja meg a webhelyek helyét.</span><span class="sxs-lookup"><span data-stu-id="64bd3-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="64bd3-121">További információért olvassa el a [webhely létrehozása a SharePoint Online-ban](https://docs.microsoft.com/sharepoint/manage-site-creation) című témakört.</span><span class="sxs-lookup"><span data-stu-id="64bd3-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

