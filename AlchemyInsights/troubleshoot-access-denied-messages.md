---
title: Hozzáférés megtagadott üzenetek hibáinak elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759802"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="6d7b1-102">Hozzáférés megtagadott üzenetek hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="6d7b1-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="6d7b1-103">Ha valaki "Hozzáférés megtagadva" üzenetet kapott egy SharePoint-mappában lévő megosztott mappához, előfordulhat, hogy a webhelycsoport rendszergazdája engedélyezte a "Korlátozott hozzáférésű felhasználói engedélyek zárolási módját".</span><span class="sxs-lookup"><span data-stu-id="6d7b1-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="6d7b1-104">A kikapcsoláshoz:</span><span class="sxs-lookup"><span data-stu-id="6d7b1-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="6d7b1-105">Tallózással keresse meg a webhelyet, kattintson a Beállítások ikonra, majd a **Webhely beállításai parancsra.**</span><span class="sxs-lookup"><span data-stu-id="6d7b1-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="6d7b1-106">A **Webhelycsoport felügyelete csoportban**kattintson **a Webhelycsoport szolgáltatásai elemre.**</span><span class="sxs-lookup"><span data-stu-id="6d7b1-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="6d7b1-107">A **Korlátozott hozzáférésű felhasználói engedélyek zárolási módja**mellett kattintson **az Inaktiválás gombra.**</span><span class="sxs-lookup"><span data-stu-id="6d7b1-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="6d7b1-108">A megosztott mappák esetében is előfordulhat hozzáférés-megtagadási üzenet, ha a webhely közzétételi webhely.</span><span class="sxs-lookup"><span data-stu-id="6d7b1-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="6d7b1-109">További információt a [Hozzáférés megtagadva megosztott mappák elérésekor (Hozzáférés megtagadva) témakörben talál.](https://go.microsoft.com/fwlink/?linkid=2004317)</span><span class="sxs-lookup"><span data-stu-id="6d7b1-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="6d7b1-110">Ha valaki "Hozzáférés megtagadva" üzenetet kapott a hozzáférési kérelmek megtekintésekor, a felhasználót webhelycsoport-rendszergazdaként vagy a webhely Tulajdonosok csoportjának tagjaként kell hozzáadni.</span><span class="sxs-lookup"><span data-stu-id="6d7b1-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="6d7b1-111">További információt a [Hozzáférés-hozzáférés-kérelmek listájában](https://go.microsoft.com/fwlink/?linkid=2004220)talál.</span><span class="sxs-lookup"><span data-stu-id="6d7b1-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="6d7b1-112">Ha egy felhasználó "Hozzáférés megtagadva" üzenetet kapott, miután eltávolították a helyszíni Active Directoryból, majd visszavették, olvassa el [a Hozzáférés megtagadva, ha egy felhasználói fiókot szinkronizál a Microsoft 365-tel.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="6d7b1-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

