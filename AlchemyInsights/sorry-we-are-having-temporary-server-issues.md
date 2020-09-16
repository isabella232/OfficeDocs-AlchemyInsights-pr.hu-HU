---
title: A Microsoft 365-alkalmazások kijavítása Sajnáljuk, mi ideiglenes kiszolgálói probléma jelenik meg
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758247"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="c6148-102">A Microsoft 365-alkalmazások rögzítése "Sajnáljuk, az ideiglenes kiszolgálói problémák merülnek fel" üzenet</span><span class="sxs-lookup"><span data-stu-id="c6148-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="c6148-103">Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="c6148-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="c6148-104">Ellenőrizze a tűzfal, a víruskereső szoftverek és a proxybeállítások között, és győződjön meg arról, hogy a Microsoft 365-alkalmazásokban nem akadályozza meg az internet elérését.</span><span class="sxs-lookup"><span data-stu-id="c6148-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="c6148-105">Lásd: [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="c6148-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="c6148-106">Nyissa meg a **Start**  >  **Run**parancsot, és írja be a **Services. msc kifejezést**.</span><span class="sxs-lookup"><span data-stu-id="c6148-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="c6148-107">Győződjön meg arról, hogy az alábbi szolgáltatások futnak:</span><span class="sxs-lookup"><span data-stu-id="c6148-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="c6148-108">Hálózati csatlakoztatott eszközök automatikus beállítása</span><span class="sxs-lookup"><span data-stu-id="c6148-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="c6148-109">Hálózati lista szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="c6148-109">Network List Service</span></span>
    - <span data-ttu-id="c6148-110">A hálózat helyének tudatosítása</span><span class="sxs-lookup"><span data-stu-id="c6148-110">Network Location Awareness</span></span>
    - <span data-ttu-id="c6148-111">Windows Eseménynapló</span><span class="sxs-lookup"><span data-stu-id="c6148-111">Windows Event Log</span></span>

<span data-ttu-id="c6148-112">Ha az egyik szolgáltatás nem fut, próbálja meg elindítani.</span><span class="sxs-lookup"><span data-stu-id="c6148-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="c6148-113">Ha probléma lép fel a szolgáltatás elindítása után, futtassa az alábbi parancsot az emelt szintű engedélyekkel rendelkező parancssor megnyitásával:</span><span class="sxs-lookup"><span data-stu-id="c6148-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="c6148-114">**sfc vizsgált**</span><span class="sxs-lookup"><span data-stu-id="c6148-114">**sfc /scannow**</span></span>

<span data-ttu-id="c6148-115">A parancs befejezése után indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="c6148-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="c6148-116">További információt az ["Sajnáljuk, nem lehet csatlakozni a fiókjához" című témakörben talál. Próbálkozzon újra később "hibaüzenet jelenik meg az aktiváláskor](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="c6148-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>