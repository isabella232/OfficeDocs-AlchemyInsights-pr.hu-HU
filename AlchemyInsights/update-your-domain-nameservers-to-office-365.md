---
title: Tartomány névkiszolgálóinak frissítése, hogy a Microsoftra irányuljanak
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734913"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="21b96-102">Tartomány névkiszolgálóinak frissítése, hogy a Microsoftra irányuljanak</span><span class="sxs-lookup"><span data-stu-id="21b96-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="21b96-103">Megjegyzés: A névkiszolgáló-módosítások elterjedéséhez néha 48 órára is szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="21b96-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="21b96-104">A tartománynak a Microsofttal való beállításához frissíteni kell a tartományregisztrálónál a névkiszolgálói szolgáltatókat.</span><span class="sxs-lookup"><span data-stu-id="21b96-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="21b96-105">Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.</span><span class="sxs-lookup"><span data-stu-id="21b96-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="21b96-106">Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.</span><span class="sxs-lookup"><span data-stu-id="21b96-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="21b96-107">Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="21b96-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="21b96-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="21b96-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="21b96-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="21b96-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="21b96-110">Mentse a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="21b96-110">Save changes.</span></span>

<span data-ttu-id="21b96-111">Ebben a cikkben részletes útmutatást talál: a [Névkiszolgálók módosítása a Microsoft 365 bármely tartományregisztrálónál való beállításához](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="21b96-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  