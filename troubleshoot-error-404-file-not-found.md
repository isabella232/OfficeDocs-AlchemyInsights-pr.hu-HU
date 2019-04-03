---
title: A fájl nem található hiba 404, – problémamegoldás
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 2b0f6d84c53b812fe0552fc05473eebdfcc8d71a
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2019
ms.locfileid: "31044042"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="28f85-102">A fájl nem található hiba 404, – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="28f85-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="28f85-103">Egy hiba 404 érkezik, amikor a felhasználók megpróbálnak hozzáférni egy webhely vagy fájl a SharePoint- vagy OneDrive.</span><span class="sxs-lookup"><span data-stu-id="28f85-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="28f85-104">Ez gyakran okozza egy webhely vagy a fájl vagy a csoport első átnevezték, törölték vagy áthelyezték.</span><span class="sxs-lookup"><span data-stu-id="28f85-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="28f85-105">Például: felhasználók próbál hozzáférni a webhelycsoport legfelső szintű 404-es hibaüzenetet fog tapasztalható, ezért törölve lett.</span><span class="sxs-lookup"><span data-stu-id="28f85-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="28f85-106">A 404-es hiba megoldása átnevezték, áthelyezték vagy törölték a webhely:</span><span class="sxs-lookup"><span data-stu-id="28f85-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="28f85-107">Klasszikus a klasszikus felügyeleti központban található helyek a [webhelycsoport törölt visszaállítása](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="28f85-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="28f85-108">Modern helyek (kommunikációs, csoporthoz csatlakozik vagy más helyek), amelyek szerepelnek az új admin center előnézetben [megtekintése és a visszaállítás törli az új SharePoint-felügyeleti központ webhelyén](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection)talál.</span><span class="sxs-lookup"><span data-stu-id="28f85-108">For modern sites (communication, group-connected, or other sites) that exist in the new admin center preview, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="28f85-109">Hiba 404, átnevezték, áthelyezték vagy törölték, a fájl (vagy más elem) megoldására:</span><span class="sxs-lookup"><span data-stu-id="28f85-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="28f85-110">Látogasson el a SharePoint- vagy OneDrive, és a Lomtárat a webhely tartalmának megjelenítése.</span><span class="sxs-lookup"><span data-stu-id="28f85-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="28f85-111">Lásd például [egy SharePoint-webhely a Lomtárban lévő elemek visszaállítása](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="28f85-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="28f85-112">Ha engedélyezve van a naplózás esetén a napló kereshet az elem kereséséhez még nem látható, [a naplófájl az Office 365 biztonsági kompatibilitási központ & keresés](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span><span class="sxs-lookup"><span data-stu-id="28f85-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
