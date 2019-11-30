---
title: Aktiválási probléma-nem tudunk csatlakozni most
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628244"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="14e16-102">Az Office-alkalmazások kijavítása "nem tudunk csatlakozni a most" üzenet</span><span class="sxs-lookup"><span data-stu-id="14e16-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="14e16-103">Ha ezt az üzenetet kapja, próbálkozzon a következőkkel:</span><span class="sxs-lookup"><span data-stu-id="14e16-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="14e16-104">Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy azok nem akadályozzák az Office alkalmazásokhoz való internet-hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="14e16-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="14e16-105">Lásd [az Office 365 URL-címeket és IP-címtartományokat](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="14e16-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="14e16-106">Megy **elkezd** > **fuss**, aztán típus **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="14e16-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="14e16-107">Ellenőrizze, hogy a következő szolgáltatások futnak-e:</span><span class="sxs-lookup"><span data-stu-id="14e16-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="14e16-108">Hálózati csatlakoztatott eszközök automatikus telepítése</span><span class="sxs-lookup"><span data-stu-id="14e16-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="14e16-109">Hálózatilista-szolgáltatás</span><span class="sxs-lookup"><span data-stu-id="14e16-109">Network List Service</span></span>
    - <span data-ttu-id="14e16-110">Hálózati helyfigyelés</span><span class="sxs-lookup"><span data-stu-id="14e16-110">Network Location Awareness</span></span>
    - <span data-ttu-id="14e16-111">Windows eseménynaplójában</span><span class="sxs-lookup"><span data-stu-id="14e16-111">Windows Event Log</span></span>

<span data-ttu-id="14e16-112">Ha az egyik ilyen szolgáltatás nem fut, próbálja meg elindítani.</span><span class="sxs-lookup"><span data-stu-id="14e16-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="14e16-113">Ha problémája van a szolgáltatás elindításával, futtassa a következő parancsot egy emelt szintű engedélyekkel rendelkező parancssorablak megnyitásával:</span><span class="sxs-lookup"><span data-stu-id="14e16-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="14e16-114">**sfc vizsgált**</span><span class="sxs-lookup"><span data-stu-id="14e16-114">**sfc /scannow**</span></span>

<span data-ttu-id="14e16-115">A parancs befejeződése után indítsa újra a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="14e16-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="14e16-116">Részletes információkért lásd: ["bocsánat, nem tudunk kapcsolódni a fiókjához. Próbálkozzon később, amikor aktiválja az Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="14e16-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>