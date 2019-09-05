---
title: SharePoint-tár leképezése hálózati meghajtóra
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: c7b16cb448684d3f68be84fda4d9de201b953ffb
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734887"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="86db8-102">SharePoint-tár leképezése hálózati meghajtóra</span><span class="sxs-lookup"><span data-stu-id="86db8-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="86db8-103">A tárak hálózati meghajtóként való hozzárendelése csak az Internet Exploreren keresztül lehetséges.</span><span class="sxs-lookup"><span data-stu-id="86db8-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="86db8-104">Alkalmanként meg kell nyitnia a SharePoint-webhelyet az Internet Explorerben, és be kell jelölnie a **Maradjon bejelentkezve** választógombot, hogy megakadályozza a munkamenet lejárása.</span><span class="sxs-lookup"><span data-stu-id="86db8-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="86db8-105">Ehelyett, [szinkronizál SharePoint fájlokat-val a új onedrive szinkronizál ügyfél](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> melyik szolgáltat [fájlokat-ra-követelés](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="86db8-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="86db8-106">Belépés minden-a fájlokat-ban OneDrive nélkül használ helyi raktározás hely.</span><span class="sxs-lookup"><span data-stu-id="86db8-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="86db8-107">Ha Ön választ-hoz leképezés egy hajt helyett [használ a új OneDrive szinkronizál ügyfél](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), biztosít Ön követ a lép az alábbi cikk.</span><span class="sxs-lookup"><span data-stu-id="86db8-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="86db8-108">**Csatlakoztatott hálózati meghajtók beállítása és hibaelhárítása**</span><span class="sxs-lookup"><span data-stu-id="86db8-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="86db8-109">Lásd: [a SharePoint onlines hálózathoz csatlakoztatott hozzárendelt hálózati meghajtók hibaelhárítása](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="86db8-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="86db8-110">Megjegyzés: Ha az Internet Explorer 10 programot Windows 8 vagy Windows 7 operációs rendszerrel használja, és a **hozzáférés megtagadva** , vagy **az elérési út nem elérhető** meghajtó leképezésekor, a [gyorsjavítás](https://support.microsoft.com/help/2846960) telepítésével oldja meg a problémát.</span><span class="sxs-lookup"><span data-stu-id="86db8-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
