---
title: Hozzáférés korlátozása a SharePoint vagy az OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750666"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8bc2b-102">Hozzáférés korlátozása a SharePoint vagy az OneDrive</span><span class="sxs-lookup"><span data-stu-id="8bc2b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8bc2b-103">A SharePoint Online/OneDrive szolgáltatásokhoz való hozzáférést sokféleképpen korlátozhatja.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="8bc2b-104">Ezek a különféle hozzáférés-korlátozási módszerek az alábbiakban kerülnek ismertetásra.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="8bc2b-105">**Engedélykorlátozás**</span><span class="sxs-lookup"><span data-stu-id="8bc2b-105">**Permission Restriction**</span></span>

<span data-ttu-id="8bc2b-106">-Ban SharePoint Online és OneDrive részére teendő, mi korlátoz belépés-hoz cikk szeret telek, fájlokat és tartók mellett egyetlen biztosít belépés-hoz azok csoportok/egyének ki kellet volna volna belépés.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="8bc2b-107">SharePoint-lista vagy-tár engedélyeinek testreszabása</span><span class="sxs-lookup"><span data-stu-id="8bc2b-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="8bc2b-108">A SharePoint-webhelyek engedélyeinek testreszabása</span><span class="sxs-lookup"><span data-stu-id="8bc2b-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="8bc2b-109">Almappára vonatkozó engedélyek módosítása</span><span class="sxs-lookup"><span data-stu-id="8bc2b-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="8bc2b-110">Nem kezelt eszközök hozzáférésének kezelése</span><span class="sxs-lookup"><span data-stu-id="8bc2b-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="8bc2b-111">Mint egy SharePoint vagy világ-admin-ban Hivatal 365, tudod fatuskó vagy korlátoz belépés-hoz SharePoint és OneDrive elégedett-ból nem kezelt berendezés (azok nem hibrid hirdetés összekapcsolt vagy szolgálatkész-ban Intune).</span><span class="sxs-lookup"><span data-stu-id="8bc2b-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="8bc2b-112">**Hálózati helykorlátozás**</span><span class="sxs-lookup"><span data-stu-id="8bc2b-112">**Network Location Restriction**</span></span>

<span data-ttu-id="8bc2b-113">A SharePoint és OneDrive erőforrásokhoz való hozzáférést az informatikai rendszergazdaként a megbízható hálózati helyek alapján szabályozhatja.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="8bc2b-114">Helyalapú házirend néven is ismert.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-114">This is also known as location-based policy.</span></span> <span data-ttu-id="8bc2b-115">További információt a [SharePoint Online és az OneDrive adataihoz való hozzáférés szabályozása a hálózati hely alapján](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="8bc2b-116">**Webhely-zárolási korlátozás**</span><span class="sxs-lookup"><span data-stu-id="8bc2b-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="8bc2b-117">A SharePoint Online szolgáltatásban lehetősége van arra, hogy zárolja a webhelygyűjteményt, így nincs hozzáférése.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="8bc2b-118">Ez a PowerShell eszközzel és a [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) segítségével állítható be, a [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate tulajdonsággal.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="8bc2b-119">**Webhelyek vagy alwebhelyek létrehozásának korlátozása a felhasználók számára**</span><span class="sxs-lookup"><span data-stu-id="8bc2b-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="8bc2b-120">A SharePoint admin vagy az Office 365 globális rendszergazda segítségével a felhasználók létrehozhatják és felügyelhetik saját SharePoint-webhelyeiket, meghatározhatják, hogy milyen webhelyeket hozhatnak létre, és meghatározhatják a webhelyek helyét.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="8bc2b-121">További információkért tekintse [meg a webhelyek létrehozásának kezelése a SharePoint Online szolgáltatásban](https://docs.microsoft.com/sharepoint/manage-site-creation) című témakört.</span><span class="sxs-lookup"><span data-stu-id="8bc2b-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

