---
title: A modern webhelyre, ahol a legfelső szintű webhely
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057723"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="8526a-102">A modern webhelyre, ahol a legfelső szintű webhely</span><span class="sxs-lookup"><span data-stu-id="8526a-102">Modern site as root site</span></span>

<span data-ttu-id="8526a-103">[Cél fontos](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) vevők most lehetővé teszi a modern kommunikációs webhely tapasztalatok a SharePoint bérlő által a klasszikus legfelső szintű helyen.</span><span class="sxs-lookup"><span data-stu-id="8526a-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="8526a-104">Ez a szolgáltatás egyszerű PowerShell parancsmag futtatásával aktiválható.</span><span class="sxs-lookup"><span data-stu-id="8526a-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="8526a-105">A PowerShell command(s) sikeres végrehajtását a legfelső szintű webhely lesz a kommunikáció új webhely kezdőlapja.</span><span class="sxs-lookup"><span data-stu-id="8526a-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="8526a-106">A cikk [Engedélyezése-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)PowerShell parancsmag és szolgáltatás követelményeiről részletesen érhetők el.</span><span class="sxs-lookup"><span data-stu-id="8526a-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="8526a-107">Azt is kell fokozatosan működés közbeni, ez ki alapértelmezés szerint célzott kiadás korai május 2019, vevőkhöz és a roll ki lesz elérhető világszerte 2019 június végén.</span><span class="sxs-lookup"><span data-stu-id="8526a-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="8526a-108">Továbbra is a [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) más új funkciókról a Modern hivatkozik.</span><span class="sxs-lookup"><span data-stu-id="8526a-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="8526a-109">**Fontos**: ne törölje a klasszikus legfelső szintű webhely a modern kommunikációs webhelyet hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="8526a-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="8526a-110">Ez a Microsoft által nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="8526a-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="8526a-111">A legfelső szintű webhely törlése tesz minden SharePoint-webhely a szervezet nem érhető el minden felhasználó számára addig, amíg a webhely visszaállítása, vagy hozzon létre egy új helyet azonos URL-címen.</span><span class="sxs-lookup"><span data-stu-id="8526a-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 