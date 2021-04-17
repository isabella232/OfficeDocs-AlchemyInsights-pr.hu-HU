---
title: Problémák a Microsoft 365-ös alkalmazásokba való bejelentkezés során
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833041"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="58f01-102">Üres bejelentkezési képernyő a Microsoft 365-alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="58f01-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="58f01-103">A probléma megoldásához próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="58f01-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="58f01-104">Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az Office legújabb [frissítéseit.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="58f01-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="58f01-105">Az Internet Explorer beállításainak alaphelyzetbe állítása: Válassza az Eszközök internetbeállítások – Az Internet Explorer beállításainak speciális alaphelyzetbe állítása lehetőséget (felhívjuk a figyelmét arra, hogy elveszíti az egyéni beállításokat), majd próbáljon meg ismét bejelentkezni az  >    >    >   Office-hoz.</span><span class="sxs-lookup"><span data-stu-id="58f01-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="58f01-106">Tiltsa le a Windows Defender alkalmazásőrt (WDAG) vagy bármely hasonló tűzfalat vagy víruskereső programot:</span><span class="sxs-lookup"><span data-stu-id="58f01-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="58f01-107">A Vezérlőpulton válassza a Programok **,** majd a **Windows-szolgáltatások be- és kikapcsolása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="58f01-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="58f01-108">Ha a Windows Defender alkalmazásőr engedélyezve van, próbálja meg letiltani.</span><span class="sxs-lookup"><span data-stu-id="58f01-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="58f01-109">**Megjegyzés:** Előfordulhat, hogy újra kell indítania a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="58f01-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="58f01-110">Győződjön meg arról, hogy a Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) beépülő modult semmilyen alkalmazás vagy tűzfal/víruskereső program nem blokkolja.</span><span class="sxs-lookup"><span data-stu-id="58f01-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="58f01-111">[Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelővel.</span><span class="sxs-lookup"><span data-stu-id="58f01-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="58f01-112">**Megjegyzés:** Az Office 2016 beállításjegyzékbeli elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="58f01-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="58f01-113">(Például: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="58f01-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="58f01-114">További információ: Csatlakozási problémák a [Windows 10-es Office 2016 16.0.7967-es](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)buildjére való frissítés után.</span><span class="sxs-lookup"><span data-stu-id="58f01-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>