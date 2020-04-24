---
title: Névkiszolgálók módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706757"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="a05a3-102">Tartomány névkiszolgálóinak frissítése, hogy a Microsoftra irányuljanak</span><span class="sxs-lookup"><span data-stu-id="a05a3-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="a05a3-103">Megjegyzés: A névkiszolgáló-módosítások elterjedéséhez néha 48 órára is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="a05a3-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="a05a3-p101">A tartománya Microsoft 365-ben való beállításához frissítenie kell a névkiszolgálói rekordokat a tartományregisztrálójánál. Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.</span><span class="sxs-lookup"><span data-stu-id="a05a3-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="a05a3-106">Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.</span><span class="sxs-lookup"><span data-stu-id="a05a3-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="a05a3-107">Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="a05a3-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="a05a3-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a05a3-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="a05a3-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a05a3-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="a05a3-110">Mentse a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="a05a3-110">Save changes.</span></span>

<span data-ttu-id="a05a3-111">Részletes útmutatást a következő cikkben talál: [A névkiszolgálók módosítása bármely tartományregisztrálónál](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="a05a3-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  