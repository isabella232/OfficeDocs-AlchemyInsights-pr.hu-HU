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
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736651"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="19e46-102">Tartomány névkiszolgálóinak frissítése az Office 365-re</span><span class="sxs-lookup"><span data-stu-id="19e46-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="19e46-103">Megjegyzés: A névkiszolgáló-módosítások elterjedéséhez néha 48 órára is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="19e46-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="19e46-p101">A tartománya Office 365-ben való beállításához frissítenie kell a névkiszolgálói rekordokat a tartományregisztrálójánál. Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.</span><span class="sxs-lookup"><span data-stu-id="19e46-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="19e46-106">Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.</span><span class="sxs-lookup"><span data-stu-id="19e46-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="19e46-107">Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="19e46-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="19e46-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="19e46-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="19e46-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="19e46-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="19e46-110">Mentse a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="19e46-110">Save changes.</span></span>

<span data-ttu-id="19e46-111">Részletes útmutatást a következő cikkben talál: [A névkiszolgálók módosítása úgy, hogy az Office 365-öt bármely tartományregisztrálónál beállíthassa](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="19e46-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  