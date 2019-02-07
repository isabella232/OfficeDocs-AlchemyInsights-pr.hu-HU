---
title: Tartomány névkiszolgálóinak frissítése az Office 365-re
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.openlocfilehash: 244997faa41bbdefc59f8096e4c23f3f4e2d5c5e
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/06/2019
ms.locfileid: "29758184"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="dc906-102">Tartomány névkiszolgálóinak frissítése az Office 365-re</span><span class="sxs-lookup"><span data-stu-id="dc906-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="dc906-103">Megjegyzés: Nameserver változások néha vehet igénybe 48 órára történő továbbításához.</span><span class="sxs-lookup"><span data-stu-id="dc906-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="dc906-p101">A tartománya Office 365-ben való beállításához frissítenie kell a névkiszolgálói rekordokat a tartományregisztrálójánál. Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.</span><span class="sxs-lookup"><span data-stu-id="dc906-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="dc906-106">Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.</span><span class="sxs-lookup"><span data-stu-id="dc906-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="dc906-107">Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="dc906-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="dc906-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="dc906-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="dc906-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="dc906-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="dc906-110">Mentse a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="dc906-110">Save changes.</span></span>
    
<span data-ttu-id="dc906-111">Részletes útmutatást a következő cikkben talál: [A névkiszolgálók módosítása úgy, hogy az Office 365-öt bármely tartományregisztrálónál beállíthassa](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="dc906-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

