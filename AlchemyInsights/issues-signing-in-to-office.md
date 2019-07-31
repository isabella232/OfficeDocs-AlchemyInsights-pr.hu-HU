---
title: Problémák az Office alkalmazások a bejelentkezés
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938239"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="17709-102">Üres bejelentkezési képernyő az Office alkalmazások</span><span class="sxs-lookup"><span data-stu-id="17709-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="17709-103">A probléma kijavításához próbálja meg a következőket:</span><span class="sxs-lookup"><span data-stu-id="17709-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="17709-104">Telepítse a legújabb frissítéseket a [Windows](https://support.microsoft.com/help/4027667/windows-10-update) és [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="17709-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="17709-105">Az Internet Explorer beállításainak alaphelyzetbe állítása: **eszközök** > **Internet-beállítások** > **Speciális** > **Internet Explorer beállításainak visszaállítása** (a Megjegyzés, hogy elveszíti az egyéni beállítások), és próbáljon új Office újra bejelentkezni.</span><span class="sxs-lookup"><span data-stu-id="17709-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="17709-106">A Windows Defender alkalmazás Guard (WDAG) vagy hasonló tűzfal vagy víruskereső programok letiltása:</span><span class="sxs-lookup"><span data-stu-id="17709-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="17709-107">A Vezérlőpulton nyissa meg a **programok**, és válassza a **Windows-szolgáltatások be- és kikapcsolása**.</span><span class="sxs-lookup"><span data-stu-id="17709-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="17709-108">Ha engedélyezve van a Windows Defender alkalmazás Guard, próbálja meg, tiltsa le.</span><span class="sxs-lookup"><span data-stu-id="17709-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="17709-109">**Megjegyzés:** Szükség lehet a számítógép újraindítására.</span><span class="sxs-lookup"><span data-stu-id="17709-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="17709-110">Győződjön meg arról, hogy a Microsoft.AAD.BrokerPlugin [Beépülő modul HRE WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne legyen blokkolva bármely alkalmazás vagy a tűzfal/anti-virus program.</span><span class="sxs-lookup"><span data-stu-id="17709-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="17709-111">[Egyértelmű Office hitelesítő adatok](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows hitelesítőadat-kezelővel.</span><span class="sxs-lookup"><span data-stu-id="17709-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="17709-112">**Megjegyzés:** A beállításjegyzék elérési utak az Office 2016 16,0 történő megváltoztak.</span><span class="sxs-lookup"><span data-stu-id="17709-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="17709-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="17709-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="17709-114">További tudnivalókért tanulmányozza a [kapcsolat problémáinak - bejelentkezés után a frissítés Office 2016 build 16.0.7967 a Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="17709-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>