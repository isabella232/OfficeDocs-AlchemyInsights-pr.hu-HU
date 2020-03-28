---
title: A SharePoint áttelepítése közbeni szabályozás
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958900"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="43d9b-102">SharePoint-szabályozás</span><span class="sxs-lookup"><span data-stu-id="43d9b-102">SharePoint throttling</span></span>

<span data-ttu-id="43d9b-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="43d9b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="43d9b-104">**A SharePoint Online szabályozása**</span><span class="sxs-lookup"><span data-stu-id="43d9b-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="43d9b-105">A SharePoint Online a szabályozást használja a SharePoint Online szolgáltatás optimális teljesítményének és megbízhatóságának fenntartásához.</span><span class="sxs-lookup"><span data-stu-id="43d9b-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="43d9b-106">A szabályozás korlátozza a felhasználói műveletek vagy a párhuzamos hívások számát (parancsprogrammal vagy kóddal) az erőforrások túlzott felhasználásának megelőzése érdekében.</span><span class="sxs-lookup"><span data-stu-id="43d9b-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="43d9b-107">További információkat az alábbi hivatkozásokon talál:</span><span class="sxs-lookup"><span data-stu-id="43d9b-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="43d9b-108">A szabályozott és a blokkolt állapot elkerülése a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="43d9b-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="43d9b-109">Adatok áttelepítése és SPO-szabályozás</span><span class="sxs-lookup"><span data-stu-id="43d9b-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="43d9b-110">A SharePoint Online- és a OneDrive-áttelepítés sebessége</span><span class="sxs-lookup"><span data-stu-id="43d9b-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="43d9b-111">A SharePoint Online-szabályozás kezelése exponenciális visszalépéssel</span><span class="sxs-lookup"><span data-stu-id="43d9b-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="43d9b-112">Kapacitástervezés és terheléstesztelés a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="43d9b-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="43d9b-113">Gyenge teljesítményt vagy szabályozást tapasztalok az áttelepítés során</span><span class="sxs-lookup"><span data-stu-id="43d9b-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)