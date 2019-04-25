---
title: Névkiszolgálók módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: ea25afd85e9ef1ae89f3a8908dc1e83a4433c890
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32394506"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e191e-102">Tartomány névkiszolgálóinak frissítése az Office 365-re</span><span class="sxs-lookup"><span data-stu-id="e191e-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e191e-103">Megjegyzés: A névkiszolgáló-módosítások elterjedéséhez néha 48 órára is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="e191e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e191e-p101">A tartománya Office 365-ben való beállításához frissítenie kell a névkiszolgálói rekordokat a tartományregisztrálójánál. Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.</span><span class="sxs-lookup"><span data-stu-id="e191e-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e191e-106">Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.</span><span class="sxs-lookup"><span data-stu-id="e191e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="e191e-107">Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="e191e-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="e191e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e191e-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="e191e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e191e-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="e191e-110">Mentse a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="e191e-110">Save changes.</span></span>
    
<span data-ttu-id="e191e-111">Részletes útmutatást a következő cikkben talál: [A névkiszolgálók módosítása úgy, hogy az Office 365-öt bármely tartományregisztrálónál beállíthassa](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="e191e-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

