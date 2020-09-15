---
title: Hozzáférés megtagadva üzenetek hibaelhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690785"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="69036-102">Hozzáférés megtagadva üzenetek hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="69036-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="69036-103">Ha valaki "hozzáférés megtagadva" üzenetet kapott egy megosztott mappához a SharePointban, előfordulhat, hogy a webhelycsoport rendszergazdája engedélyezte a "korlátozott hozzáférésű felhasználói engedély zárolási üzemmódját" jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="69036-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="69036-104">A funkció kikapcsolása:</span><span class="sxs-lookup"><span data-stu-id="69036-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="69036-105">Tallózással keresse meg a webhelyet, kattintson a Beállítások ikonra, majd a **webhely beállításai**parancsra.</span><span class="sxs-lookup"><span data-stu-id="69036-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="69036-106">A webhelycsoport **felügyelete**csoportban kattintson a webhelycsoport **szolgáltatásai**hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="69036-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="69036-107">A **korlátozott hozzáférésű felhasználói engedély zárolási üzemmódja**mellett kattintson az **inaktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="69036-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="69036-108">Ha a webhely közzétételi webhelye, a megosztott mappákhoz hozzáférés-megtagadási üzenet is előfordulhat.</span><span class="sxs-lookup"><span data-stu-id="69036-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="69036-109">További információ: [hozzáférés megtagadva egy megosztott mappa elérésekor](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="69036-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="69036-110">Ha valaki "hozzáférés megtagadva" üzenetet kapott a hozzáférési kérelmek megtekintésekor, a felhasználót a webhelycsoport rendszergazdája vagy a webhely tulajdonosok csoportjának tagjaként kell hozzáadnia.</span><span class="sxs-lookup"><span data-stu-id="69036-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="69036-111">További információt a [hozzáférés megtagadva a hozzáférési kérelmek listájához](https://go.microsoft.com/fwlink/?linkid=2004220)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="69036-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="69036-112">Ha egy felhasználó "hozzáférés megtagadva" üzenetet kapott, miután eltávolítottak őket a helyszíni Active Directoryból, majd újból hozzáadta őket, tekintse át a [hozzáférés megtagadva, ha a felhasználói fiók szinkronizálva van a Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)-val.</span><span class="sxs-lookup"><span data-stu-id="69036-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

