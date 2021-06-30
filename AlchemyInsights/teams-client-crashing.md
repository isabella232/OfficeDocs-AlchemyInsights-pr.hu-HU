---
title: Teams ügyfél összeomlik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187723"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="19aa4-102">Teams ügyfél összeomlik</span><span class="sxs-lookup"><span data-stu-id="19aa4-102">Teams client crashing</span></span>

<span data-ttu-id="19aa4-103">Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="19aa4-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="19aa4-104">Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="19aa4-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="19aa4-105">Győződjön meg arról, hogy a [Microsoft 365 összes URL-címe és címtartománya](/microsoftteams/connectivity-issues) elérhető.</span><span class="sxs-lookup"><span data-stu-id="19aa4-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="19aa4-106">Jelentkezzen be a bérlőhöz tartozó rendszergazdai fiókjával, és a [Szolgáltatásállapot irányítópultot](/office365/enterprise/view-service-health) ellenőrizve győződjön meg arról, hogy nincs kimaradás vagy teljesítménycsökkenés a szolgáltatás működésében.</span><span class="sxs-lookup"><span data-stu-id="19aa4-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="19aa4-107">A telepített alkalmazás Teams újratelepítése</span><span class="sxs-lookup"><span data-stu-id="19aa4-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="19aa4-108">Tallózással keresse meg a számítógépen az %appdata%\Microsoft\Teams\ mappát, és törölje a címtárban lévő összes fájlt.</span><span class="sxs-lookup"><span data-stu-id="19aa4-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="19aa4-109">[Töltse le és telepítse az Teams alkalmazást](https://www.microsoft.com/microsoft-teams/download-app), és ha lehetséges, telepítse az Teams alkalmazást rendszergazdaként  (kattintson a jobb gombbal a Teams telepítőjére, és válassza a Futtatás rendszergazdaként lehetőséget, ha elérhető).</span><span class="sxs-lookup"><span data-stu-id="19aa4-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="19aa4-110">Ha az Teams továbbra is összeomlik, próbálja meg reprodukálni a problémát.</span><span class="sxs-lookup"><span data-stu-id="19aa4-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="19aa4-111">Ha van rá szükség:</span><span class="sxs-lookup"><span data-stu-id="19aa4-111">If you can:</span></span>

1. <span data-ttu-id="19aa4-112">A Problémarögzítő használatával rögzítse az elvégzett lépéseket.</span><span class="sxs-lookup"><span data-stu-id="19aa4-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="19aa4-113">Zárja be az ÖSSZES szükségtelen vagy bizalmas alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="19aa4-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="19aa4-114">Indítsa el a Problémarögzítőt, és reprodukálja a problémát úgy, hogy közben az érintett felhasználói fiókkal van bejelentkezve.</span><span class="sxs-lookup"><span data-stu-id="19aa4-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="19aa4-115">[Gyűjtse össze a rögzített reprodukálási lépéseket tartalmazó Teams-naplókat](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="19aa4-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="19aa4-116">**Megjegyzés**: Ügyeljen arra, hogy rögzítse az érintett felhasználó bejelentkezési címét.</span><span class="sxs-lookup"><span data-stu-id="19aa4-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="19aa4-117">Gyűjtse össze a memóriaképek és/vagy hibagyűjtők adatait (Windows).</span><span class="sxs-lookup"><span data-stu-id="19aa4-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="19aa4-118">Indítsa Windows Powershellt a gépen, ahol az összeomlás történik, és futtassa az alábbi parancsokat (az egyes parancsok után nyomja le az Enter billentyűt):</span><span class="sxs-lookup"><span data-stu-id="19aa4-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="19aa4-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="19aa4-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="19aa4-120">Miután létrehozott egy szövegfájlt, és megjelent a képernyőn, mentse a fájlt, és csatolja a szolgáltatáskéréshez.</span><span class="sxs-lookup"><span data-stu-id="19aa4-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
