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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030581"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a29d6-102">Összeomlik a Teams ügyfélprogram?</span><span class="sxs-lookup"><span data-stu-id="a29d6-102">Teams client crashing?</span></span>

<span data-ttu-id="a29d6-103">Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="a29d6-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a29d6-104">Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a29d6-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a29d6-105">Győződjön meg arról, hogy az [Office 365 URL-címei és címtartományai](https://docs.microsoft.com/microsoftteams/connectivity-issues) elérhetők.</span><span class="sxs-lookup"><span data-stu-id="a29d6-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a29d6-106">Jelentkezzen be a rendszergazdai fiókjával, és a [Szolgáltatásállapot irányítópultot](https://docs.microsoft.com/office365/enterprise/view-service-health) ellenőrizve erősítse meg, hogy nincs kimaradás vagy szolgáltatásiteljesítmény-csökkenés.</span><span class="sxs-lookup"><span data-stu-id="a29d6-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="a29d6-107">Utolsó lépésként megpróbálhatja törölni a Teams ügyféloldali gyorsítótárát:</span><span class="sxs-lookup"><span data-stu-id="a29d6-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="a29d6-108">Lépjen ki teljesen a Microsoft Teams asztali ügyfélprogramból.</span><span class="sxs-lookup"><span data-stu-id="a29d6-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="a29d6-109">Kattinthat a jobb gombbal a **Teams** ikonjára az ikontálcán, majd a **Kilépés** parancsra, illetve futtathatja a Feladatkezelőt, és teljesen leállíthatja a folyamatot.</span><span class="sxs-lookup"><span data-stu-id="a29d6-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="a29d6-110">Nyissa meg a Fájlkezelőt, és írja be a következőt: %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="a29d6-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="a29d6-111">A könyvtárban az alábbi mappák közül látható néhány:</span><span class="sxs-lookup"><span data-stu-id="a29d6-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="a29d6-112">Az **alkalmazás-gyorsítótáron** belül nyissa meg a gyorsítótárat, és törölje a fájlok bármelyikét a gyorsítótár helyén: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="a29d6-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="a29d6-113">A **blobtárolóban** törölje az összes fájlt: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="a29d6-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="a29d6-114">A **gyorsítótárban** törölje az összes fájlt: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="a29d6-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="a29d6-115">Az **adatbázisokban** törölje az összes fájlt: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="a29d6-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="a29d6-116">Az **GPU-gyorsítótárban** törölje az összes fájlt: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="a29d6-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="a29d6-117">Az **IndexedDB**, helyen törölje a .db fájlt: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="a29d6-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="a29d6-118">A **helyi tárhelyen** törölje az összes fájlt: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="a29d6-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="a29d6-119">Végül a **tmp** könyvtárban törölje bármelyik fájlt: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="a29d6-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="a29d6-120">Indítsa újra a Teams ügyfélprogramot.</span><span class="sxs-lookup"><span data-stu-id="a29d6-120">Restart your Teams client.</span></span>
