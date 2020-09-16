---
title: A 404 hibáinak elhárítása, a fájl nem található
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: e76864949bde7230e63f509823ab1e3edf631388
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750093"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="2e674-102">A 404 hibáinak elhárítása, a fájl nem található</span><span class="sxs-lookup"><span data-stu-id="2e674-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="2e674-103">404-es hibaüzenetet kap, amikor a felhasználók megkísérelnek hozzáférni egy webhelyhez vagy fájlhoz a SharePointban vagy a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2e674-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="2e674-104">Ezt gyakran okozhatja a átnevezni, áthelyezni vagy törölni kívánt webhely vagy csoport.</span><span class="sxs-lookup"><span data-stu-id="2e674-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="2e674-105">Például: a felhasználók a legfelső szintű webhelycsoport eléréséhez szükséges 404-hibát tapasztalnak, és törölték.</span><span class="sxs-lookup"><span data-stu-id="2e674-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="2e674-106">Az 404-es kódú hiba elhárítása átnevezve, áthelyezve vagy törölték:</span><span class="sxs-lookup"><span data-stu-id="2e674-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="2e674-107">A klasszikus felügyeleti központban megtalálható klasszikus webhelyekről a [törölt webhelycsoport visszaállítása](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)című témakörben tájékozódhat.</span><span class="sxs-lookup"><span data-stu-id="2e674-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="2e674-108">Az új SharePoint felügyeleti központban megtalálható modern webhelyekhez (kommunikációhoz, csoporthoz kapcsolt vagy más webhelyekhez) lásd [a törölt webhelyek megtekintése és visszaállítása az új SharePoint felügyeleti központban](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)című témakört.</span><span class="sxs-lookup"><span data-stu-id="2e674-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="2e674-109">Az 404 hibájának elhárítása, amelyet átneveztek, áthelyeztek vagy töröltek:</span><span class="sxs-lookup"><span data-stu-id="2e674-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="2e674-110">Nyissa meg a SharePoint-vagy OneDrive webhelyet, és tekintse meg a Lomtár webhelyet a webhely tartalmából.</span><span class="sxs-lookup"><span data-stu-id="2e674-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="2e674-111">Lásd: a [SharePoint-webhely Lomtárában lévő elemek visszaállítása](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="2e674-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="2e674-112">Ha továbbra sem találja azt az elemet, amelyet a naplózás engedélyezésekor meg tud keresni, keresse meg a naplót [a Microsoft 365 biztonsági & megfelelőségi központban](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="2e674-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
