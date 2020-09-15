---
title: '404-es kódú hiba: a fájl nem található'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d8e0d855e1e5fe702d468c0a4075a6f3264e67c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709225"
---
# <a name="error-404-file-not-found-in-sharepoint-or-onedrive"></a><span data-ttu-id="f814d-102">404-as kódú hiba: a fájl nem található a SharePointban vagy a OneDrive-ban</span><span class="sxs-lookup"><span data-stu-id="f814d-102">Error 404: File not found in SharePoint or OneDrive</span></span>

<span data-ttu-id="f814d-103">**404-as kódú hiba: a fájl nem található** , amikor a felhasználók megkísérelnek hozzáférni egy webhelyhez vagy fájlhoz a SharePointban vagy a OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f814d-103">**Error 404: File not found** is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="f814d-104">Ezt gyakran okozhatja a átnevezni, áthelyezni vagy törölni kívánt webhely vagy csoport.</span><span class="sxs-lookup"><span data-stu-id="f814d-104">This is often caused by a site or file or group getting renamed, moved, or deleted.</span></span>
<span data-ttu-id="f814d-105">A felhasználók megtapasztalják a hibát, amikor megkísérelnek hozzáférni a legfelső szintű webhelycsoporthoz, és törölték.</span><span class="sxs-lookup"><span data-stu-id="f814d-105">Users will experience the error when attempting to access the root site collection and it has been deleted.</span></span>

<span data-ttu-id="f814d-106">Az alábbi segíthet a probléma megoldásában:</span><span class="sxs-lookup"><span data-stu-id="f814d-106">The following can help with resolving this issue:</span></span>
- <span data-ttu-id="f814d-107">Az [új SharePoint felügyeleti központban megtekintheti és visszaállíthatja a törölt webhelyeket](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center): az új felügyeleti központ előzetes verziójában megtalálhatók a modern webhelyek (például a kommunikáció, a csoporttal összekapcsolt vagy más webhelyek).</span><span class="sxs-lookup"><span data-stu-id="f814d-107">[View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center):  For modern sites (communication, group-connected, or other sites) that exist in the new admin center preview.</span></span>
- <span data-ttu-id="f814d-108">A [SharePoint-webhely Lomtárában lévő elemek visszaállítása](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be): az áthelyezett vagy törölt fájlok (vagy egyéb elemek) feloldásához nyissa meg a SharePoint-vagy OneDrive-webhelyet, és tekintse meg a Lomtár tartalmát a webhely tartalmából.</span><span class="sxs-lookup"><span data-stu-id="f814d-108">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be):  To resolve file (or other item) that has been renamed, moved or deleted go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span>
- <span data-ttu-id="f814d-109">[Keresés a naplóban a biztonság &amp; területén Megfelelőségi központ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance): Keresés a naplóban (ha engedélyezve van a naplózás) Ha továbbra sem találja az elemet.</span><span class="sxs-lookup"><span data-stu-id="f814d-109">[Search the audit log in the Security &amp; Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance):  Search the audit log (if logging is enabled) if you are still unable to find the item.</span></span>