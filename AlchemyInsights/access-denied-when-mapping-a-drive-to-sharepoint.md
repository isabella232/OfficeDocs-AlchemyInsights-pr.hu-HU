---
title: Hozzáférés megtagadva, ha a meghajtó hozzárendelése SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 2e37c936d1b908729fe870f13ba6c60047c655c3
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473589"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="892e1-102">SharePoint-tárak csatlakoztatott hálózati meghajtókhoz problémáit</span><span class="sxs-lookup"><span data-stu-id="892e1-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="892e1-103">A csatlakoztatott hálózati meghajtók tallózásakor megjelenhet a következő üzenetek valamelyikét:</span><span class="sxs-lookup"><span data-stu-id="892e1-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="892e1-104">**\\Elérési út nem érhető el. Lehet, hogy nincs engedélye a hálózati erőforrás használatához. Forduljon a rendszergazdához annak megállapításához, ha a hozzáférési engedélyeket kell a kiszolgáló.**</span><span class="sxs-lookup"><span data-stu-id="892e1-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>
    
- <span data-ttu-id="892e1-105">**A hozzáférés megtagadva. Mielőtt megnyitná a fájlt ezen a helyen, meg kell először adja hozzá a webhelyet a megbízható helyek listájához, tallózással keresse meg a webhelyet, és válassza az automatikus bejelentkezési lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="892e1-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>
    
<span data-ttu-id="892e1-106">A [get-help hibaelhárítás csatlakoztatott hálózati meghajtók](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx).</span><span class="sxs-lookup"><span data-stu-id="892e1-106">[Get help troubleshooting mapped network drives](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx).</span></span>
  
<span data-ttu-id="892e1-p101">A dokumentumtár hálózati meghajtóként leképezése szolgáltatás, ideiglenes, és csak az Internet Explorer támogatott. Ehelyett [Új ügyfél OneDrive szinkronizálása a SharePoint-fájlok szinkronizálása](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) tartalmazó [Fájlok igény](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). OneDrive az összes fájl elérhető helyi tárolóhely használata nélkül.</span><span class="sxs-lookup"><span data-stu-id="892e1-p101">Mapping a library as a network drive is temporary and supported only in Internet Explorer. Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Access all your files in OneDrive without using local storage space.</span></span>
  

