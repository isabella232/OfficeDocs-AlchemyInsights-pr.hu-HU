---
title: Az Exchange PowerShell és az egyszerű hitelesítés elévülése
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813474"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="0ac9e-102">Az Exchange PowerShell és az egyszerű hitelesítés elévülése</span><span class="sxs-lookup"><span data-stu-id="0ac9e-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="0ac9e-103">Ha további információra van szüksége arról, hogy miként csatlakozhat az Exchange Online PowerShellhez egyszerű hitelesítés használata nélkül, [látogasson el ide](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="0ac9e-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="0ac9e-104">A PowerShell V2 modul nem használ egyszerű hitelesítést.</span><span class="sxs-lookup"><span data-stu-id="0ac9e-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="0ac9e-105">Felhívjuk a figyelmét arra, hogy az egyszerű hitelesítésnek továbbra is engedélyezve kell lennie az ügyfélgépen.</span><span class="sxs-lookup"><span data-stu-id="0ac9e-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="0ac9e-106">Az új PowerShell V2 modul modern hitelesítés használatával létesít kapcsolatot, hogy lehetővé tegye az összes REST-alapú V2-es parancsmag használatát.</span><span class="sxs-lookup"><span data-stu-id="0ac9e-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="0ac9e-107">A V2-es parancsmagok használata mellett ez azt is lehetővé teszi, hogy elérjék a régebbi Távoli PowerShell-parancsmagokat (RPS), amelyekhez Távoli PowerShell-munkamenetet kell létesíteni.</span><span class="sxs-lookup"><span data-stu-id="0ac9e-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="0ac9e-108">Ahhoz, hogy RPS-munkamenetet létesítsenek Windows rendszerű gépen, a WinRM egyszerű hitelesítésnek engedélyezve kell lennie az ügyfélgépen annak ellenére, hogy a modul modern hitelesítési mechanizmust használ a szolgáltatás felé történő hitelesítéshez.</span><span class="sxs-lookup"><span data-stu-id="0ac9e-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="0ac9e-109">A rendszer a WinRM egyszerű hitelesítés csatornáját használja a modern hitelesítés jogkivonatainak továbbítására.</span><span class="sxs-lookup"><span data-stu-id="0ac9e-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="0ac9e-110">Ha a WinRM egyszerű hitelesítés le van tiltva az ügyfélgépen, az új V2-es parancsmagok továbbra is működni fognak (a régebbi RPS-parancsmagok azonban nem).</span><span class="sxs-lookup"><span data-stu-id="0ac9e-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
