---
title: A hozzáférés megtagadva üzenetet – problémamegoldás
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473023"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="0df03-102">A hozzáférés megtagadva üzenetet – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="0df03-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="0df03-p101">Ha valaki kapott egy "Hozzáférés megtagadva" üzenetet egy megosztott mappába, a webhelycsoport rendszergazdája valószínűleg engedélyezte "korlátozott hozzáférésű felhasználói engedély zárolási mód." Kapcsolja ki ezt:</span><span class="sxs-lookup"><span data-stu-id="0df03-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="0df03-105">Tallózással keresse meg a webhelyet, kattintson a beállítások ikonra, és kattintson a **Webhely beállításai**.</span><span class="sxs-lookup"><span data-stu-id="0df03-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="0df03-106">**Helycsoport felügyelete**csoportban kattintson a **webhelycsoport-szolgáltatások**.</span><span class="sxs-lookup"><span data-stu-id="0df03-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="0df03-107">**Korlátozott hozzáférésű felhasználói engedély zárolási mód**mellett kattintson az **Inaktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="0df03-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="0df03-p102">Ha a webhely a közzététel során a hozzáférés megtagadva üzenetet is előfordulhat a megosztott mappák. Info tanulmányozza a [Megosztott mappák elérése hozzáférés megtagadva](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="0df03-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="0df03-p103">Ha egy valaki kapott egy "Hozzáférés megtagadva" üzenetet megjeleníteni a hozzáférési kérelmeket, a felhasználónak kell hozzá kell adni a webhelycsoport rendszergazdája vagy a webhelyet a tulajdonosok csoport tagjai. További információért lásd a [Hozzáférési kérelmek listához a hozzáférés megtagadva](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="0df03-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="0df03-112">Ha a felhasználó egy "Hozzáférés megtagadva" üzenetet kapott, voltak helyszíni Active Directory eltávolítja és ismét hozzáadja, lásd: [Hozzáférés megtagadva az Office 365 felhasználói fiókkal szinkronizálható](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="0df03-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

