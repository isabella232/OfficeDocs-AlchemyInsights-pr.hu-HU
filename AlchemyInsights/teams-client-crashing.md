---
title: Összeomlik a Teams ügyfélprogram?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354054"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a31c0-102">Összeomlik a Teams ügyfélprogram?</span><span class="sxs-lookup"><span data-stu-id="a31c0-102">Teams client crashing?</span></span>

<span data-ttu-id="a31c0-103">Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="a31c0-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a31c0-104">Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a31c0-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a31c0-105">Győződjön meg arról, hogy a [Microsoft 365 összes URL-címe és címtartománya](https://docs.microsoft.com/microsoftteams/connectivity-issues) elérhető.</span><span class="sxs-lookup"><span data-stu-id="a31c0-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a31c0-106">Jelentkezzen be a bérlői rendszergazdai fiókkal, és ellenőrizze a [Szolgáltatásállapot-irányítópultot,](https://docs.microsoft.com/office365/enterprise/view-service-health) és ellenőrizze, hogy nincs-e kimaradás vagy szolgáltatáslebontás.</span><span class="sxs-lookup"><span data-stu-id="a31c0-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="a31c0-107">A Teams alkalmazás eltávolítása és újratelepítése (hivatkozás)</span><span class="sxs-lookup"><span data-stu-id="a31c0-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="a31c0-108">Tallózással keresse meg a számítógép %appdata%\Microsoft\teams\ mappáját, és törölje a könyvtár összes fájlját.</span><span class="sxs-lookup"><span data-stu-id="a31c0-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="a31c0-109">[Töltse le és telepítse a Teams alkalmazást,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)és ha lehetséges, telepítse a Teamst rendszergazdaként (kattintson a jobb gombbal a Teams telepítőjére, és ha elérhető, válassza a "Futtatás rendszergazdaként" lehetőséget).</span><span class="sxs-lookup"><span data-stu-id="a31c0-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="a31c0-110">Ha a Teams-ügyfél még mindig összeomlik, reprodukálhatja a problémát?</span><span class="sxs-lookup"><span data-stu-id="a31c0-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="a31c0-111">Ha igen:</span><span class="sxs-lookup"><span data-stu-id="a31c0-111">If so:</span></span>

1. <span data-ttu-id="a31c0-112">A lépésrögzítő vel rögzítheti a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="a31c0-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="a31c0-113">Zárja be az összes felesleges vagy bizalmas alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="a31c0-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="a31c0-114">Indítsa el a Lépésrögzítőt, és reprodukálja a problémát, miközben bejelentkezik az érintett felhasználói fiókkal.</span><span class="sxs-lookup"><span data-stu-id="a31c0-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="a31c0-115">[Gyűjtse össze a csapatok naplókat, hogy rögzítse a rögzített repro lépéseket](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="a31c0-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="a31c0-116">**Megjegyzés:** Győződjön meg arról, hogy rögzíti az érintett felhasználó bejelentkezési címét.</span><span class="sxs-lookup"><span data-stu-id="a31c0-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="a31c0-117">Gyűjtse össze a memóriakép és/vagy a Hibagyűjtő adatait (Windows).</span><span class="sxs-lookup"><span data-stu-id="a31c0-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="a31c0-118">Indítsa el a Windows Powershell t azon a számítógépen, amelyen az összeomlás történik, és futtassa a következő parancsokat:</span><span class="sxs-lookup"><span data-stu-id="a31c0-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="a31c0-119">Csatolja a fájlt a támogatási esethez.</span><span class="sxs-lookup"><span data-stu-id="a31c0-119">Attach the file to your support case.</span></span>
