---
title: A PowerShell önkiszolgáló vásárlása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091713"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="0dabb-102">A PowerShell önkiszolgáló vásárlása</span><span class="sxs-lookup"><span data-stu-id="0dabb-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="0dabb-103">Az MSCommerce PowerShell modul használatához telepítenie kell azt egy TLS 1.2-es (helyi rendszergazdai engedélyekkel rendelkező) Windows 10-es eszközre.</span><span class="sxs-lookup"><span data-stu-id="0dabb-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="0dabb-104">Importálja és csatlakozzon az MSCommerce modulhoz.</span><span class="sxs-lookup"><span data-stu-id="0dabb-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="0dabb-105">Amikor a rendszer kéri a bejelentkezést, globális vagy számlázási rendszergazdai szerepkör hitelesítő adatait kell használnia.</span><span class="sxs-lookup"><span data-stu-id="0dabb-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="0dabb-106">Ha nem rendelkezik TLS 1.2-vel, a következő hibaüzenet jelenhet meg a házirend betöltésekor vagy frissítésekor:</span><span class="sxs-lookup"><span data-stu-id="0dabb-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="0dabb-107">*ErrorMessage -Az alapul szolgáló kapcsolat megszakadt: Váratlan hiba történt a küldéssorán.*</span><span class="sxs-lookup"><span data-stu-id="0dabb-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



