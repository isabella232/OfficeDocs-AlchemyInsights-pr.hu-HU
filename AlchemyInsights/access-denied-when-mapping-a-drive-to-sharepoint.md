---
title: Hozzáférés megtagadva, amikor egy meghajtót SharePoint-hoz képez
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 23ee86df5404b6f20f3a4b605038b31b6f9fd731
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687368"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="60c67-102">A hálózati meghajtókra leképezett SharePoint-tárakkal kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="60c67-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="60c67-103">Amikor leképezett hálózati meghajtót tallóz, az alábbi üzenetek egyike jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="60c67-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="60c67-104">**\\Az elérési út nem érhető el. Lehet, hogy nincs engedélye a hálózati erőforrás használatára. Lépjen kapcsolatba a kiszolgáló rendszergazdájával, és érdeklődjön, hogy rendelkezik-e hozzáférési engedélyekkel.**</span><span class="sxs-lookup"><span data-stu-id="60c67-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="60c67-105">**Hozzáférés megtagadva. Mielőtt fájlokat nyitna meg ezen a helyen, először hozzá kell adnia a webhelyet a megbízható helyek listájához, meg kell tallóznia a webhelyre, és ki kell választania az automatikus bejelentkezés lehetőségét.**</span><span class="sxs-lookup"><span data-stu-id="60c67-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="60c67-106">[Segítség a leképezett hálózati meghajtók kal kapcsolatos hibaelhárításhoz.](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="60c67-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="60c67-107">A tár hálózati meghajtóként való hozzárendelése ideiglenes, és csak az Internet Explorer ben támogatott.</span><span class="sxs-lookup"><span data-stu-id="60c67-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="60c67-108">Ehelyett [szinkronizálja a SharePoint-fájlokat az új OneDrive szinkronizálási ügyfélalkalmazással,](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) amely tartalmazza [az igény szerinti fájlokat.](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)</span><span class="sxs-lookup"><span data-stu-id="60c67-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="60c67-109">A OneDrive-on lévő összes fájlját a helyi tárhely használata nélkül érheti el.</span><span class="sxs-lookup"><span data-stu-id="60c67-109">Access all your files in OneDrive without using local storage space.</span></span>
  