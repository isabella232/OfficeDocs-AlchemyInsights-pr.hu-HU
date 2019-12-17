---
title: A Megnyitás Intézővel paranccsal kapcsolatos hibák elhárítása a SharePoint Online-ban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 21a0c193b752342d47189dda73d171249153f7fc
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050815"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="a7cd7-102">A Megnyitás Intézővel paranccsal kapcsolatos hibák elhárítása a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="a7cd7-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="a7cd7-103">A Megnyitás Intézővel parancs megnyitja a Windows Intéző egy helyi példányát, amely a SharePoint webhely kiszolgálójának mappaszerkezetét jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="a7cd7-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="a7cd7-104">Ezért javasoljuk, hogy [a SharePoint-fájlok szinkronizálását a OneDrive új szinkronizálási ügyfelével,](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> amely az [Igény szerinti fájlok](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) funkcióval helyi hozzáférést biztosít a fájlokhoz, és a legjobb teljesítményt nyújtja.</span><span class="sxs-lookup"><span data-stu-id="a7cd7-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="a7cd7-105">Ha úgy dönt, hogy az új OneDrive szinkronizálási ügyfél helyett a Tallózó nézetet használja, kövesse a következő cikkben leírt lépéseket és gyakorlati tanácsokat:</span><span class="sxs-lookup"><span data-stu-id="a7cd7-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="a7cd7-106">A „Megnyitás Intézővel“ parancs használata a SharePoint Online-ban előforduló hibák elhárításához</span><span class="sxs-lookup"><span data-stu-id="a7cd7-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="a7cd7-107">Tárban lévő fájlok másolása vagy áthelyezése a Megnyitás Intézővel parancs használatával</span><span class="sxs-lookup"><span data-stu-id="a7cd7-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="a7cd7-108">A **Megnyitás Intézővel** gomb nem jelenik meg az új tár felületén.</span><span class="sxs-lookup"><span data-stu-id="a7cd7-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="a7cd7-109">Kattintson a jobb felső sarokban lévő **Nézet** legördülő menüre (a legördülő menü neve az aktuális nézettől függően változik), majd válassza a **Megtekintés Fájlkezelőben elemet**.</span><span class="sxs-lookup"><span data-stu-id="a7cd7-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="a7cd7-110">A SharePoint Megnyitás Intézővel parancsa ActiveX-vezérlőket használ, ezért az csak az Internet Explorer 10-es vagy 11-es verziójában támogatott.</span><span class="sxs-lookup"><span data-stu-id="a7cd7-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="a7cd7-111">A Megnyitás Intézővel parancs nem használható a Windowsban a Microsoft Edge, a Google Chrome, a Mozilla Firefox böngészővel, illetve a Mac platformon.</span><span class="sxs-lookup"><span data-stu-id="a7cd7-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="a7cd7-112">Emiatt előfordulhat, hogy a Tallózó nézet beállítás szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="a7cd7-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="a7cd7-113">[Miért nem érhetők el vagy szürkék a gombok a SharePoint menüszalagján?](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="a7cd7-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

