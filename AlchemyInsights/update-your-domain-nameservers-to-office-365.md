---
title: A tartománynév-kiszolgálók frissítése a Microsoft ra
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719995"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="5c60b-102">A tartománynév-kiszolgálók frissítése a Microsoft ra</span><span class="sxs-lookup"><span data-stu-id="5c60b-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="5c60b-103">Megjegyzés: A névkiszolgáló-módosítások elterjedéséhez néha 48 órára is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="5c60b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="5c60b-104">A tartomány Microsofttal való beállításához frissíteni kell a regisztráló névkiszolgálóit.</span><span class="sxs-lookup"><span data-stu-id="5c60b-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="5c60b-105">Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.</span><span class="sxs-lookup"><span data-stu-id="5c60b-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="5c60b-106">Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.</span><span class="sxs-lookup"><span data-stu-id="5c60b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="5c60b-107">Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="5c60b-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="5c60b-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5c60b-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="5c60b-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5c60b-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="5c60b-110">Mentse a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="5c60b-110">Save changes.</span></span>

<span data-ttu-id="5c60b-111">A cikkben részletes utasításokat is talál: [A névkiszolgálók módosítása a Microsoft 365 beállításához bármely tartományregisztrálóval](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="5c60b-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  