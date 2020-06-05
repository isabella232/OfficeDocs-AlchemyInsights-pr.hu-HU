---
title: Problémák a Microsoft 365-alkalmazásokba való bejelentkezéssel kapcsolatban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579903"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="fde1a-102">Üres bejelentkezési képernyő a Microsoft 365-alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="fde1a-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="fde1a-103">A probléma megoldásához próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="fde1a-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="fde1a-104">Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="fde1a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="fde1a-105">Az Internet Explorer beállításainak alaphelyzetbe állítása: Nyissa meg **az**  >  **Internetbeállítások –**  >  **Internet**Explorer  >  **beállításainak alaphelyzetbe állítása** lehetőséget (vegye figyelembe, hogy az egyéni beállítások elvesznek), majd próbáljon meg újra bejelentkezni az Office-ba.</span><span class="sxs-lookup"><span data-stu-id="fde1a-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="fde1a-106">Tiltsa le a Windows Defender Application Guard (WDAG) vagy bármely hasonló tűzfal at vagy víruskereső programot:</span><span class="sxs-lookup"><span data-stu-id="fde1a-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="fde1a-107">A Vezérlőpulton nyissa meg a **Programok**lapot, és válassza **a Windows-szolgáltatások be- és kikapcsolása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="fde1a-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="fde1a-108">Ha a Windows Defender Alkalmazásvédő engedélyezve van, próbálja meg letiltani.</span><span class="sxs-lookup"><span data-stu-id="fde1a-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="fde1a-109">**Megjegyzés:** Lehet, hogy újra kell indítania a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="fde1a-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="fde1a-110">Győződjön meg arról, hogy a Microsoft.AAD.BrokerPlugin [AAD WAM beépülő modult](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) semmilyen alkalmazás vagy tűzfal/víruskereső program nem blokkolja.</span><span class="sxs-lookup"><span data-stu-id="fde1a-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="fde1a-111">[Az Office hitelesítő adatainak törlése a](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítő adatok kezelőjével</span><span class="sxs-lookup"><span data-stu-id="fde1a-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="fde1a-112">**Megjegyzés:** Az Office 2016 beállításjegyzék-elérési útjai 16.0-ra változtak.</span><span class="sxs-lookup"><span data-stu-id="fde1a-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fde1a-113">(Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="fde1a-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="fde1a-114">További információt a [Csatlakozási problémák a Bejelentkezési problémák az Office 2016 16.0.7967-es frissítése után Windows 10 rendszeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="fde1a-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>