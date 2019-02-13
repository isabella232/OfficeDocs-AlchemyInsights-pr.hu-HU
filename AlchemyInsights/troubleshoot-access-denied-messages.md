---
title: A hozzáférés megtagadva üzenetet – problémamegoldás
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916454"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="34e73-102">A hozzáférés megtagadva üzenetet – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="34e73-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="34e73-p101">Ha valaki kapott egy "Hozzáférés megtagadva" üzenetet egy megosztott mappába, a webhelycsoport rendszergazdája valószínűleg engedélyezte "korlátozott hozzáférésű felhasználói engedély zárolási mód." Kapcsolja ki ezt:</span><span class="sxs-lookup"><span data-stu-id="34e73-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="34e73-105">Tallózással keresse meg a webhelyet, kattintson a beállítások ikonra, és kattintson a **Webhely beállításai**.</span><span class="sxs-lookup"><span data-stu-id="34e73-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="34e73-106">**Helycsoport felügyelete**csoportban kattintson a **webhelycsoport-szolgáltatások**.</span><span class="sxs-lookup"><span data-stu-id="34e73-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="34e73-107">**Korlátozott hozzáférésű felhasználói engedély zárolási mód**mellett kattintson az **Inaktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="34e73-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="34e73-p102">Ha a webhely a közzététel során a hozzáférés megtagadva üzenetet is előfordulhat a megosztott mappák. Info tanulmányozza a [Megosztott mappák elérése hozzáférés megtagadva](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="34e73-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="34e73-p103">Ha egy valaki kapott egy "Hozzáférés megtagadva" üzenetet megjeleníteni a hozzáférési kérelmeket, a felhasználónak kell hozzá kell adni a webhelycsoport rendszergazdája vagy a webhelyet a tulajdonosok csoport tagjai. További információért lásd a [Hozzáférési kérelmek listához a hozzáférés megtagadva](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="34e73-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="34e73-112">Ha a felhasználó egy "Hozzáférés megtagadva" üzenetet kapott, voltak helyszíni Active Directory eltávolítja és ismét hozzáadja, lásd: [Hozzáférés megtagadva az Office 365 felhasználói fiókkal szinkronizálható](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="34e73-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

