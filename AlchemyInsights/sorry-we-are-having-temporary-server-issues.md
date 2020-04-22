---
title: Az Office-alkalmazások javítása Elnézést, ideiglenes kiszolgálói problémák üzenettel kapcsolatosak
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764119"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="b4358-102">Az Office-alkalmazások javítása "Sajnáljuk, ideiglenes kiszolgálóproblémák vannak" üzenet</span><span class="sxs-lookup"><span data-stu-id="b4358-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="b4358-103">Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="b4358-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b4358-104">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e az Office-alkalmazások internet-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="b4358-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="b4358-105">Lásd [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b4358-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b4358-106">Nyissa meg a**Futtatás** **indítása** > , majd írja be **a services.msc**.</span><span class="sxs-lookup"><span data-stu-id="b4358-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b4358-107">Győződjön meg arról, hogy a következő szolgáltatások futnak:</span><span class="sxs-lookup"><span data-stu-id="b4358-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b4358-108">Hálózati csatlakoztatott eszközök automatikus beállítása</span><span class="sxs-lookup"><span data-stu-id="b4358-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b4358-109">Hálózati lista szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="b4358-109">Network List Service</span></span>
    - <span data-ttu-id="b4358-110">Hálózati helyfigyelés</span><span class="sxs-lookup"><span data-stu-id="b4358-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b4358-111">Windows eseménynapló</span><span class="sxs-lookup"><span data-stu-id="b4358-111">Windows Event Log</span></span>

<span data-ttu-id="b4358-112">Ha a szolgáltatások egyike nem fut, próbálja meg elindítani.</span><span class="sxs-lookup"><span data-stu-id="b4358-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b4358-113">Ha problémája van a szolgáltatás elindításával, futtassa a következő parancsot egy emelt szintű engedélyekkel rendelkező parancssor megnyitásával:</span><span class="sxs-lookup"><span data-stu-id="b4358-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b4358-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="b4358-114">**sfc /scannow**</span></span>

<span data-ttu-id="b4358-115">A parancs befejezése után indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="b4358-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b4358-116">A részletes információt a ["Sajnáljuk, nem tudunk csatlakozni a fiókjához" című témakörben talál. Próbálkozzon később" hibaüzenet jelenik meg az aktiváláskor.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="b4358-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>