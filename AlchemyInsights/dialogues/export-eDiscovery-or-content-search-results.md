---
title: EDiscovery/Content Search eredmények exportálása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429603"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="26146-102">EDiscovery/Content Search eredmények exportálása</span><span class="sxs-lookup"><span data-stu-id="26146-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="26146-103">Előfordulhat, hogy a keresési eredményeket EGY PST-fájlba (e-mailből) vagy natív Office-dokumentumokba kell exportálni (SharePoint- és OneDrive Vállalati verziós webhelyekről).</span><span class="sxs-lookup"><span data-stu-id="26146-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="26146-104">Ha igen, tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="26146-104">If so, do the following:</span></span>

- <span data-ttu-id="26146-105">Győződjön meg arról, hogy fiókja rendelkezik az exportáláshoz szükséges megfelelő engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="26146-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="26146-106">További információt a "Elektronikus adatok [kiosztási engedélyének" kiosztása lapon láthat.](https://go.microsoft.com/fwlink/?linkid=2102406)</span><span class="sxs-lookup"><span data-stu-id="26146-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="26146-107">Győződjön meg arról, hogy számítógépe megfelelt az összes [előfeltételnek.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="26146-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="26146-108">Nem minden böngésző támogatott, például a Chrome.</span><span class="sxs-lookup"><span data-stu-id="26146-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="26146-109">Exportálás tartalomkeresésből: a.</span><span class="sxs-lookup"><span data-stu-id="26146-109">To export from a Content Search: a.</span></span> <span data-ttu-id="26146-110">Keresse fel [a Biztonsági & megfelelőségi](https://protection.office.com/contentsearch) központot, kattintson a Keresés elemre, majd válassza a **Tartalomkeresés lehetőséget.** </span><span class="sxs-lookup"><span data-stu-id="26146-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="26146-111">A **Tartalomkeresés lapon** jelöljön ki egy mentett keresést.</span><span class="sxs-lookup"><span data-stu-id="26146-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="26146-112">b.</span><span class="sxs-lookup"><span data-stu-id="26146-112">b.</span></span> <span data-ttu-id="26146-113">A Részletek ablaktábla **Eredmények exportálása számítógépre** parancsa alatt válassza az Exportálás **elkezdése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="26146-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="26146-114">Ha több mint 100 000 000 postaládát exportál, az exportálási eredmények letöltéséhez a PowerShellt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="26146-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="26146-115">További információt a több mint [100 000 000](https://go.microsoft.com/fwlink/?linkid=2143861)postaláda eredményeinek exportálása.</span><span class="sxs-lookup"><span data-stu-id="26146-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="26146-116">További információ: [Tartalomkeresési eredmények exportálása.](https://go.microsoft.com/fwlink/?linkid=2102118)</span><span class="sxs-lookup"><span data-stu-id="26146-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>