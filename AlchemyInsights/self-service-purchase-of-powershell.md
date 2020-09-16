---
title: A PowerShell önkiszolgáló vásárlása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739972"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="c6e29-102">A PowerShell önkiszolgáló vásárlása</span><span class="sxs-lookup"><span data-stu-id="c6e29-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="c6e29-103">A MSCommerce PowerShell-modul használatához telepítenie kell azt Windows 10-es eszközön a TLS 1,2 (szükséges helyi rendszergazdai engedélyekkel).</span><span class="sxs-lookup"><span data-stu-id="c6e29-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="c6e29-104">Importálás és csatlakozás a MSCommerce modulhoz.</span><span class="sxs-lookup"><span data-stu-id="c6e29-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="c6e29-105">Amikor a rendszer arra kéri, hogy jelentkezzen be, globális vagy számlázási rendszergazdai szerepkör-hitelesítő adatokat kell használnia.</span><span class="sxs-lookup"><span data-stu-id="c6e29-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="c6e29-106">Ha nincs TLS 1,2, a következő hibaüzenet jelenhet meg a házirend beszerzése vagy frissítése során:</span><span class="sxs-lookup"><span data-stu-id="c6e29-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="c6e29-107">*ErrorMessage – az alapul szolgáló kapcsolat bezárult: váratlan hiba történt a küldésben*.</span><span class="sxs-lookup"><span data-stu-id="c6e29-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



