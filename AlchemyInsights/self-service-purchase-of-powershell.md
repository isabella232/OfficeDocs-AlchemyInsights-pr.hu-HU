---
title: A PowerShell önkiszolgáló megvásárlása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797723"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="97819-102">A PowerShell önkiszolgáló megvásárlása</span><span class="sxs-lookup"><span data-stu-id="97819-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="97819-103">Az MSCommerce PowerShell modult TLS 1.2-es TLS 1.2-es Windows 10-es eszközre kell telepítenie (helyi rendszergazdai engedélyek szükségesek).</span><span class="sxs-lookup"><span data-stu-id="97819-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="97819-104">Importálja az MSCommerce modult, és csatlakozzon ahhoz.</span><span class="sxs-lookup"><span data-stu-id="97819-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="97819-105">Amikor a rendszer arra kéri, hogy jelentkezzen be, a globális vagy számlázási rendszergazdai szerepkörhöz szükséges hitelesítő adatokat kell használnia.</span><span class="sxs-lookup"><span data-stu-id="97819-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="97819-106">Ha nem TLS 1.2-es, a következő hibaüzenet jelenhet meg, amikor megkísérli be szerezni vagy frissíteni a házirendet:</span><span class="sxs-lookup"><span data-stu-id="97819-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="97819-107">*ErrorMessage – A mögöttes kapcsolat lezárult: Váratlan* hiba történt egy küldésen.</span><span class="sxs-lookup"><span data-stu-id="97819-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



