---
title: Az Exchange PowerShell és az egyszerű hitelesítés elévülése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015691"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="b2e24-102">Az Exchange PowerShell és az egyszerű hitelesítés elévülése</span><span class="sxs-lookup"><span data-stu-id="b2e24-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="b2e24-103">Ha további információra van szüksége arról, hogy miként csatlakozhat az Exchange Online PowerShellhez egyszerű hitelesítés használata nélkül, [látogasson el ide](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="b2e24-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="b2e24-104">Felhívjuk a figyelmét arra, hogy az egyszerű hitelesítésnek továbbra is engedélyezve kell lennie az ügyfélgépen.</span><span class="sxs-lookup"><span data-stu-id="b2e24-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="b2e24-105">Az új PowerShell V2 modul modern hitelesítés használatával létesít kapcsolatot, hogy lehetővé tegye az összes REST-alapú V2-es parancsmag használatát.</span><span class="sxs-lookup"><span data-stu-id="b2e24-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="b2e24-106">A V2-es parancsmagok használata mellett ez azt is lehetővé teszi, hogy elérjék a régebbi Távoli PowerShell-parancsmagokat (RPS), amelyekhez Távoli PowerShell-munkamenetet kell létesíteni.</span><span class="sxs-lookup"><span data-stu-id="b2e24-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="b2e24-107">Ahhoz, hogy RPS-munkamenetet létesítsenek Windows rendszerű gépen, a WinRM egyszerű hitelesítésnek engedélyezve kell lennie az ügyfélgépen annak ellenére, hogy a modul modern hitelesítési mechanizmust használ a szolgáltatás felé történő hitelesítéshez.</span><span class="sxs-lookup"><span data-stu-id="b2e24-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="b2e24-108">A rendszer a WinRM egyszerű hitelesítés csatornáját használja a modern hitelesítés jogkivonatainak továbbítására.</span><span class="sxs-lookup"><span data-stu-id="b2e24-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="b2e24-109">Ha a WinRM egyszerű hitelesítés le van tiltva az ügyfélgépen, az új V2-es parancsmagok továbbra is működni fognak (a régebbi RPS-parancsmagok azonban nem).</span><span class="sxs-lookup"><span data-stu-id="b2e24-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
