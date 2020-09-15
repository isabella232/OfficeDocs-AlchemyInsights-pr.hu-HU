---
title: A Microsoft 365 alkalmazásba való bejelentkezéssel kapcsolatos problémák
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695289"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="8ec6b-102">Üres bejelentkezési képernyő a Microsoft 365-alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="8ec6b-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="8ec6b-103">A probléma megoldásához próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="8ec6b-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="8ec6b-104">Telepítse a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és az [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="8ec6b-105">Az Internet Explorer beállításainak visszaállítása: nyissa **meg az Internet**  >  Explorer**Beállítások**  >  **speciális**  >  **visszaállítása** (ne feledje, hogy az egyéni beállítások törlődnek), majd próbáljon meg ismét bejelentkezni az Office-ba.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="8ec6b-106">Tiltsa le a Windows Defender alkalmazás-Gárda (WDAG) vagy más hasonló tűzfal-vagy víruskereső programját:</span><span class="sxs-lookup"><span data-stu-id="8ec6b-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="8ec6b-107">A Vezérlőpulton kattintson a **programok**elemre, majd **a Windows-szolgáltatások be-és kikapcsolása**elemre.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="8ec6b-108">Ha a Windows Defender alkalmazás-Gárda engedélyezve van, próbálja meg letiltani.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="8ec6b-109">**Megjegyzés:** Lehet, hogy újra kell indítania a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="8ec6b-110">Győződjön meg arról, hogy a Microsoft. AAD. BrokerPlugin [aad a WAM beépülő modult](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) semmilyen alkalmazás vagy tűzfal/víruskereső program letiltja.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="8ec6b-111">[Törölje az Office-hitelesítő adatokat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) a Windows Hitelesítőadat-kezelő használatával.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="8ec6b-112">**Megjegyzés:** Az Office-2016 rendszerleíró elérési útja megváltozott a 16,0-ra.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8ec6b-113">(Pl.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="8ec6b-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="8ec6b-114">További információ: bejelentkezés az [Office 2016-hoz Windows 10 rendszerre való frissítés után a bejelentkezéskor jelentkező kapcsolódási problémákkal](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="8ec6b-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>