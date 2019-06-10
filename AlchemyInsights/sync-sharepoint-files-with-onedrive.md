---
title: SharePoint-fájlok szinkronizálása a OneDrive új szinkronizálási ügyfelével
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757817"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="43aa9-102">SharePoint-fájlok szinkronizálása a OneDrive új szinkronizálási ügyfelével</span><span class="sxs-lookup"><span data-stu-id="43aa9-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="43aa9-103">A Megnyitás Intézővel parancs megnyitja a Windows Intéző egy helyi példányát, amely a SharePoint webhely kiszolgálójának mappaszerkezetét jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="43aa9-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="43aa9-104">Ezért javasoljuk [a SharePoint-fájlok szinkronizálását a OneDrive új szinkronizálási ügyfelével,](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> amely az [Igény szerinti fájlok](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) funkcióval helyi hozzáférést biztosít a fájlokhoz, és a legjobb teljesítményt nyújtja.</span><span class="sxs-lookup"><span data-stu-id="43aa9-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="43aa9-105">Ha úgy dönt, hogy az új szinkronizálási ügyfél helyett a Tallózó nézetet használja, kövesse az alábbi cikkben leírt lépéseket és gyakorlati tanácsokat.</span><span class="sxs-lookup"><span data-stu-id="43aa9-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="43aa9-106">A „Megnyitás Intézővel“ parancs használata a SharePoint Online-ban előforduló hibák elhárításához</span><span class="sxs-lookup"><span data-stu-id="43aa9-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- <span data-ttu-id="43aa9-107">[Tárban lévő fájlok másolása vagy áthelyezése a Megnyitás Intézővel parancs használatával](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="43aa9-107">See [Video: Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2).</span></span>

<span data-ttu-id="43aa9-108">Megjegyzés: A Megnyitás Intézővel gomb nem jelenik meg az új tár felületén.</span><span class="sxs-lookup"><span data-stu-id="43aa9-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="43aa9-109">Kattintson a jobb felső sarokban lévő Nézet legördülő menüre (a legördülő menü neve az aktuális nézettől függően változik), majd a Fájlkezelőben a Nézet elemre.</span><span class="sxs-lookup"><span data-stu-id="43aa9-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="43aa9-110">A SharePoint Megnyitás Intézővel parancsa ActiveX-vezérlőket használ, ezért az csak az Internet Explorer 10-es vagy 11-es verziójában támogatott.</span><span class="sxs-lookup"><span data-stu-id="43aa9-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="43aa9-111">A Megnyitás Intézővel parancs nem használható a Windowsban a Microsoft Edge, a Google Chrome, a Mozilla Firefox böngészővel, illetve a Mac platformon.</span><span class="sxs-lookup"><span data-stu-id="43aa9-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="43aa9-112">Emiatt előfordulhat, hogy a Tallózó nézet beállítás szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="43aa9-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="43aa9-113">[Miért nem érhetők el vagy szürkék a gombok a SharePoint menüszalagján?](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="43aa9-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

