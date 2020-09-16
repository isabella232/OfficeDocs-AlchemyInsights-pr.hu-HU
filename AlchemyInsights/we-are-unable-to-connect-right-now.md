---
title: Aktiválási probléma – jelenleg nem tudunk csatlakozni
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725985"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="ac53e-102">A Microsoft 365-alkalmazások rögzítése "a kapcsolat most nem érhető el" üzenet</span><span class="sxs-lookup"><span data-stu-id="ac53e-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="ac53e-103">Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="ac53e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ac53e-104">Ellenőrizze a tűzfal, a víruskereső szoftverek és a proxybeállítások között, és győződjön meg arról, hogy a Microsoft 365-alkalmazásokban nem akadályozza meg az internet elérését.</span><span class="sxs-lookup"><span data-stu-id="ac53e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="ac53e-105">Lásd: [Microsoft URL-EK és IP-](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)címtartományok.</span><span class="sxs-lookup"><span data-stu-id="ac53e-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ac53e-106">Nyissa meg a **Start**  >  **Run**parancsot, és írja be a **Services. msc kifejezést**.</span><span class="sxs-lookup"><span data-stu-id="ac53e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ac53e-107">Győződjön meg arról, hogy az alábbi szolgáltatások futnak:</span><span class="sxs-lookup"><span data-stu-id="ac53e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ac53e-108">Hálózati csatlakoztatott eszközök automatikus beállítása</span><span class="sxs-lookup"><span data-stu-id="ac53e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ac53e-109">Hálózati lista szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="ac53e-109">Network List Service</span></span>
    - <span data-ttu-id="ac53e-110">A hálózat helyének tudatosítása</span><span class="sxs-lookup"><span data-stu-id="ac53e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ac53e-111">Windows Eseménynapló</span><span class="sxs-lookup"><span data-stu-id="ac53e-111">Windows Event Log</span></span>

<span data-ttu-id="ac53e-112">Ha az egyik szolgáltatás nem fut, próbálja meg elindítani.</span><span class="sxs-lookup"><span data-stu-id="ac53e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ac53e-113">Ha probléma lép fel a szolgáltatás elindítása után, futtassa az alábbi parancsot az emelt szintű engedélyekkel rendelkező parancssor megnyitásával:</span><span class="sxs-lookup"><span data-stu-id="ac53e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ac53e-114">**sfc vizsgált**</span><span class="sxs-lookup"><span data-stu-id="ac53e-114">**sfc /scannow**</span></span>

<span data-ttu-id="ac53e-115">A parancs befejezése után indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="ac53e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ac53e-116">További információt az ["Sajnáljuk, nem lehet csatlakozni a fiókjához" című témakörben talál. Próbálkozzon újra később "hibaüzenet jelenik meg, amikor aktiválja az Office-t a Microsoft 365-ből](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ac53e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>