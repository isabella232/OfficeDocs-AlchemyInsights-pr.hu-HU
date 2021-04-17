---
title: A Microsoft 365-ös appok kijavítása Sajnáljuk, átmeneti kiszolgáló-problémákról következő üzenet jelenik meg
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835273"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="a818b-102">A Microsoft 365-alkalmazások "Sajnáljuk, ideiglenes kiszolgáló-problémákat tudunk" üzenetének kijavítása</span><span class="sxs-lookup"><span data-stu-id="a818b-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="a818b-103">Ha megjelenik ez az üzenet, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="a818b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a818b-104">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem gátolja meg a Microsoft 365-alkalmazásokhoz való internet-hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="a818b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a818b-105">Lásd: [URL-ek és IP-címtartományok.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="a818b-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a818b-106">Válassza a **Start**  >  **Run ot,** majd írja be a **services.msc parancsot.**</span><span class="sxs-lookup"><span data-stu-id="a818b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a818b-107">Győződjön meg arról, hogy az alábbi szolgáltatások mind futnak:</span><span class="sxs-lookup"><span data-stu-id="a818b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a818b-108">Hálózati eszközök automatikus beállítása</span><span class="sxs-lookup"><span data-stu-id="a818b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a818b-109">Hálózati lista szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="a818b-109">Network List Service</span></span>
    - <span data-ttu-id="a818b-110">Hálózati hely tájékoztatása</span><span class="sxs-lookup"><span data-stu-id="a818b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a818b-111">Windows eseménynapló</span><span class="sxs-lookup"><span data-stu-id="a818b-111">Windows Event Log</span></span>

<span data-ttu-id="a818b-112">Ha a szolgáltatások egyike nem fut, próbálja meg elindítani.</span><span class="sxs-lookup"><span data-stu-id="a818b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a818b-113">Ha problémát okoz a szolgáltatás indítása, futtassa a következő parancsot egy magasabb szintű engedélyekkel rendelkező parancssor megnyitásával:</span><span class="sxs-lookup"><span data-stu-id="a818b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a818b-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="a818b-114">**sfc /scannow**</span></span>

<span data-ttu-id="a818b-115">A parancs befejezését követően indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="a818b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a818b-116">Részletes információkért lásd: "Sajnáljuk, nem lehet [csatlakozni a fiókjához. Kérjük, próbálkozzon újra később" hibaüzenet jelenik meg az aktiváláskor.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="a818b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>