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
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500408"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="b087f-102">A hozzáférés megtagadva üzenetet – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="b087f-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="b087f-103">Ha valaki kapott egy "Hozzáférés megtagadva" üzenetet egy megosztott mappába, a SharePoint, a webhelycsoport rendszergazdája valószínűleg engedélyezte "korlátozott hozzáférésű felhasználói engedély zárolási mód."</span><span class="sxs-lookup"><span data-stu-id="b087f-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="b087f-104">Kapcsolja ki ezt:</span><span class="sxs-lookup"><span data-stu-id="b087f-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="b087f-105">Tallózással keresse meg a webhelyet, kattintson a beállítások ikonra, és kattintson a **Webhely beállításai**.</span><span class="sxs-lookup"><span data-stu-id="b087f-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="b087f-106">**Helycsoport felügyelete**csoportban kattintson a **webhelycsoport-szolgáltatások**.</span><span class="sxs-lookup"><span data-stu-id="b087f-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="b087f-107">**Korlátozott hozzáférésű felhasználói engedély zárolási mód**mellett kattintson az **Inaktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="b087f-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="b087f-108">Ha a webhely a közzététel során a hozzáférés megtagadva üzenetet is előfordulhat a megosztott mappák.</span><span class="sxs-lookup"><span data-stu-id="b087f-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="b087f-109">Info tanulmányozza a [Megosztott mappák elérése hozzáférés megtagadva](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="b087f-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="b087f-110">Ha egy valaki kapott egy "Hozzáférés megtagadva" üzenetet megjeleníteni a hozzáférési kérelmeket, a felhasználónak kell hozzá kell adni a webhelycsoport rendszergazdája vagy a webhelyet a tulajdonosok csoport tagjai.</span><span class="sxs-lookup"><span data-stu-id="b087f-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="b087f-111">További információért lásd a [Hozzáférési kérelmek listához a hozzáférés megtagadva](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="b087f-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="b087f-112">Ha a felhasználó egy "Hozzáférés megtagadva" üzenetet kapott, voltak helyszíni Active Directory eltávolítja és ismét hozzáadja, lásd: [Hozzáférés megtagadva az Office 365 felhasználói fiókkal szinkronizálható](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="b087f-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

