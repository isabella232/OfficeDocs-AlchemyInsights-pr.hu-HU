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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704896"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="59b37-102">Hozzáférés megtagadva üzenetek hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="59b37-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="59b37-103">Ha valaki "Hozzáférés megtagadva" üzenetet kapott egy Megosztott mappába a SharePointban, előfordulhat, hogy a webhelycsoport rendszergazdája engedélyezte a "Korlátozott hozzáférésű felhasználói engedély zárolási mód" beállítást.</span><span class="sxs-lookup"><span data-stu-id="59b37-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="59b37-104">A következőt kapcsolhatja ki:</span><span class="sxs-lookup"><span data-stu-id="59b37-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="59b37-105">Tallózással keresse meg a webhelyet, kattintson a Beállítások ikonra, majd a **Webhely beállításai elemre.**</span><span class="sxs-lookup"><span data-stu-id="59b37-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="59b37-106">A **Webhelycsoport felügyelete alatt kattintson** a **Webhelycsoport-szolgáltatások elemre.**</span><span class="sxs-lookup"><span data-stu-id="59b37-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="59b37-107">A Korlátozott **hozzáférésű felhasználói** engedély zárolási módja mellett kattintson az Inaktiválás **gombra.**</span><span class="sxs-lookup"><span data-stu-id="59b37-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="59b37-108">A "Hozzáférés megtagadva" üzenet megosztott mappák esetén is előfordulhat, ha a webhely közzétételi webhely.</span><span class="sxs-lookup"><span data-stu-id="59b37-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="59b37-109">További információért lásd: [Hozzáférés megtagadva megosztott mappa elérésekor.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="59b37-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="59b37-110">Ha valaki "Hozzáférés megtagadva" üzenetet kapott a hozzáférési kérelmek megtekintésekor, a felhasználót fel kell véve webhelycsoport-rendszergazdaként vagy a Tulajdonosok csoport tagjaként a webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="59b37-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="59b37-111">További információért lásd: Hozzáférés megtagadva a hozzáférési [kérelmek listájához.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="59b37-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="59b37-112">Ha egy felhasználó "Hozzáférés megtagadva" üzenetet kapott, miután eltávolította a helyszíni Active Directoryból, majd hozzáadta őket, a Hozzáférés megtagadva, amikor egy felhasználói fiók szinkronizálódik [a Microsoft 365-be.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="59b37-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

