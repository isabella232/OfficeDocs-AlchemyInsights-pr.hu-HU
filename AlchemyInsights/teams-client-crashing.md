---
title: Összeomlik a Teams ügyfélprogram?
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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826273"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="cc666-102">Összeomlik a Teams ügyfélprogram?</span><span class="sxs-lookup"><span data-stu-id="cc666-102">Teams client crashing?</span></span>

<span data-ttu-id="cc666-103">Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="cc666-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="cc666-104">Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="cc666-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="cc666-105">Győződjön meg arról, hogy a [Microsoft 365 összes URL-címe és címtartománya](https://docs.microsoft.com/microsoftteams/connectivity-issues) elérhető.</span><span class="sxs-lookup"><span data-stu-id="cc666-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="cc666-106">Jelentkezzen be a bérlőhöz tartozó rendszergazdai fiókjával, és a [Szolgáltatásállapot irányítópultot](https://docs.microsoft.com/office365/enterprise/view-service-health) ellenőrizve győződjön meg arról, hogy nincs kimaradás vagy teljesítménycsökkenés a szolgáltatás működésében.</span><span class="sxs-lookup"><span data-stu-id="cc666-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="cc666-107">Távolítsa el, majd telepítse újra a Teams alkalmazást (hivatkozás).</span><span class="sxs-lookup"><span data-stu-id="cc666-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="cc666-108">Tallózással nyissa meg a számítógépen az %appdata%\Microsoft\teams\ mappát, és törölje a benne lévő összes fájlt.</span><span class="sxs-lookup"><span data-stu-id="cc666-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="cc666-109">[Töltse le és telepítse a Teams alkalmazást](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), és lehetőség szerint rendszergazdaként végezze el a Teams telepítését (kattintson a jobb gombbal a Teams telepítőjére, és válassza a „Futtatás rendszergazdaként” menüpontot, ha elérhető).</span><span class="sxs-lookup"><span data-stu-id="cc666-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="cc666-110">Ha a Teams ügyfélprogram továbbra is összeomlik, reprodukálható a probléma?</span><span class="sxs-lookup"><span data-stu-id="cc666-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="cc666-111">Ha igen:</span><span class="sxs-lookup"><span data-stu-id="cc666-111">If so:</span></span>

1. <span data-ttu-id="cc666-112">A Problémarögzítő használatával rögzítse az elvégzett lépéseket.</span><span class="sxs-lookup"><span data-stu-id="cc666-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="cc666-113">Zárja be az ÖSSZES szükségtelen vagy bizalmas alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="cc666-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="cc666-114">Indítsa el a Problémarögzítőt, és reprodukálja a problémát úgy, hogy közben az érintett felhasználói fiókkal van bejelentkezve.</span><span class="sxs-lookup"><span data-stu-id="cc666-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="cc666-115">[Gyűjtse össze a rögzített reprodukálási lépéseket tartalmazó Teams-naplókat](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="cc666-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="cc666-116">**Megjegyzés**: Ügyeljen arra, hogy rögzítse az érintett felhasználó bejelentkezési címét.</span><span class="sxs-lookup"><span data-stu-id="cc666-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="cc666-117">Gyűjtse össze a memóriaképek és/vagy hibagyűjtők adatait (Windows).</span><span class="sxs-lookup"><span data-stu-id="cc666-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="cc666-118">Indítsa el a Windows PowerShellt azon a gépen, amelyen az összeomlás előfordul, és futtassa az alábbi parancsokat:</span><span class="sxs-lookup"><span data-stu-id="cc666-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="cc666-119">Csatolja a fájlt a támogatási esethez.</span><span class="sxs-lookup"><span data-stu-id="cc666-119">Attach the file to your support case.</span></span>
