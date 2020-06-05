---
title: A Microsoft 365-alkalmazások javítása Elnézést, ideiglenes kiszolgálói problémáküzenettel állunk
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582705"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="6f0b0-102">A Microsoft 365 alkalmazások javítása "Sajnáljuk, ideiglenes kiszolgálóproblémákkal kapcsolatos problémák vannak" üzenet</span><span class="sxs-lookup"><span data-stu-id="6f0b0-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="6f0b0-103">Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="6f0b0-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6f0b0-104">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e a Microsoft 365-alkalmazások internet-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="6f0b0-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="6f0b0-105">Lásd [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6f0b0-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="6f0b0-106">Nyissa **Start**meg a  >  **Futtatás**indítása , majd írja be **a services.msc**.</span><span class="sxs-lookup"><span data-stu-id="6f0b0-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="6f0b0-107">Győződjön meg arról, hogy a következő szolgáltatások futnak:</span><span class="sxs-lookup"><span data-stu-id="6f0b0-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="6f0b0-108">Hálózati csatlakoztatott eszközök automatikus beállítása</span><span class="sxs-lookup"><span data-stu-id="6f0b0-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="6f0b0-109">Hálózati lista szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="6f0b0-109">Network List Service</span></span>
    - <span data-ttu-id="6f0b0-110">Hálózati helyfigyelés</span><span class="sxs-lookup"><span data-stu-id="6f0b0-110">Network Location Awareness</span></span>
    - <span data-ttu-id="6f0b0-111">Windows eseménynapló</span><span class="sxs-lookup"><span data-stu-id="6f0b0-111">Windows Event Log</span></span>

<span data-ttu-id="6f0b0-112">Ha a szolgáltatások egyike nem fut, próbálja meg elindítani.</span><span class="sxs-lookup"><span data-stu-id="6f0b0-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="6f0b0-113">Ha problémája van a szolgáltatás elindításával, futtassa a következő parancsot egy emelt szintű engedélyekkel rendelkező parancssor megnyitásával:</span><span class="sxs-lookup"><span data-stu-id="6f0b0-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="6f0b0-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="6f0b0-114">**sfc /scannow**</span></span>

<span data-ttu-id="6f0b0-115">A parancs befejezése után indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="6f0b0-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="6f0b0-116">A részletes információt a ["Sajnáljuk, nem tudunk csatlakozni a fiókjához" című témakörben talál. Próbálkozzon később" hibaüzenet jelenik meg az aktiváláskor.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="6f0b0-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>