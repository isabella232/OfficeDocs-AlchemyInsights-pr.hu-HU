---
title: A SharePoint Online szabályozása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773849"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="88b85-102">A SharePoint Online szabályozása</span><span class="sxs-lookup"><span data-stu-id="88b85-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="88b85-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="88b85-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="88b85-104">**a 503-kiszolgáló foglalt hiba**</span><span class="sxs-lookup"><span data-stu-id="88b85-104">**503 server is busy error**</span></span>

<span data-ttu-id="88b85-105">A felhasználók a SharePoint-vagy a OneDrive-webhelyeken való navigáláskor elfoglalt hibába ütközhet a 503-kiszolgálóval.</span><span class="sxs-lookup"><span data-stu-id="88b85-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="88b85-106">Ezt a hibát a SharePoint-szolgáltatáson belüli szabályozás okozhatja.</span><span class="sxs-lookup"><span data-stu-id="88b85-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="88b85-107">A SharePoint Online a szabályozást használja a SharePoint Online szolgáltatás optimális teljesítményének és megbízhatóságának fenntartásához.</span><span class="sxs-lookup"><span data-stu-id="88b85-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="88b85-108">A szabályozás korlátozza a felhasználói műveletek vagy a párhuzamos hívások számát (parancsprogrammal vagy kóddal) az erőforrások túlzott felhasználásának megelőzése érdekében.</span><span class="sxs-lookup"><span data-stu-id="88b85-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="88b85-109">A szabályozással kapcsolatos további tudnivalókért olvassa el a [SharePoint Online-ban a letiltott vagy Letiltva](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="88b85-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="88b85-110">Ha úgy véli, hogy ez a hiba nem kapcsolódik a szabályozáshoz, ellenőrizheti, hogy a bérlői webhelyre való navigáláskor van-e aktív [karbantartás.](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="88b85-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="88b85-111">Végül győződjön meg róla, hogy felkeresi a [szolgáltatás állapota](https://portal.office.com/adminportal/home#/servicehealth) lapot, és ellenőrizheti, hogy milyen figyelmeztetésekkel/incidensekkel fordulhat elő.</span><span class="sxs-lookup"><span data-stu-id="88b85-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

