---
title: Hozzáférés-megtagadási üzenetek – problémamegoldás
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050707"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="44ce8-102">Hozzáférés-megtagadási üzenetek – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="44ce8-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="44ce8-103">Ha valaki "hozzáférés megtagadva" üzenetet kapott a SharePoint rendszerben lévő megosztott mappához, előfordulhat, hogy a webhelycsoport rendszergazdája engedélyezte a "korlátozott hozzáférésű felhasználói engedélyek zárolási módját".</span><span class="sxs-lookup"><span data-stu-id="44ce8-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="44ce8-104">Kikapcsolásához:</span><span class="sxs-lookup"><span data-stu-id="44ce8-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="44ce8-105">Tallózással keresse meg a webhelyet, kattintson a Beállítások ikonra, majd kattintson a **webhely beállításai**lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="44ce8-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="44ce8-106">A **Webhelycsoport felügyelete**csoportban kattintson a **webhelycsoport-szolgáltatások**elemre.</span><span class="sxs-lookup"><span data-stu-id="44ce8-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="44ce8-107">A **korlátozott hozzáférésű felhasználói engedély zárolási módja**mellett kattintson az **inaktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="44ce8-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="44ce8-108">A hozzáférés megtagadva üzenetek akkor is előfordulhatnak a megosztott mappákban, ha a webhely közzétételi webhely.</span><span class="sxs-lookup"><span data-stu-id="44ce8-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="44ce8-109">További információ a [hozzáférés megtagadva a megosztott mappához való hozzáféréskor](https://go.microsoft.com/fwlink/?linkid=2004317)című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="44ce8-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="44ce8-110">Ha valaki hozzáférés-megtagadási üzenetet kapott a hozzáférési kérelmek megtekintésekor, akkor a felhasználót webhelycsoport-rendszergazdaként vagy a webhely tulajdonosok csoportjának egy tagaként kell hozzáadni.</span><span class="sxs-lookup"><span data-stu-id="44ce8-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="44ce8-111">További információért olvassa el a hozzáférési [kérelmek listájának hozzáférés megtagadva](https://go.microsoft.com/fwlink/?linkid=2004220)című témakört.</span><span class="sxs-lookup"><span data-stu-id="44ce8-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="44ce8-112">Ha egy felhasználó "hozzáférés megtagadva" üzenetet kapott, miután eltávolították őket az Active Directory címtárból, majd hozzáadta a biztonsági másolatot, akkor olvassa el [a hozzáférés megtagadva választógombot, amikor egy felhasználói fiók szinkronizálva van az Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="44ce8-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

