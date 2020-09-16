---
title: Összeomlást okozó hibák elhárítása OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665000"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="446c7-102">Összeomlást okozó hibák elhárítása OneDrive</span><span class="sxs-lookup"><span data-stu-id="446c7-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="446c7-103">Ha a OneDrive ismétlődően összeomlik, próbálkozzon az alábbi hibaelhárítási lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="446c7-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="446c7-104">**Győződjön meg arról, hogy a rendszerleíró kulcsok nem állíthatók be:**</span><span class="sxs-lookup"><span data-stu-id="446c7-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="446c7-105">A Rendszerleíróadatbázis-szerkesztő segítségével keresse meg a HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="446c7-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="446c7-106">Ha a DisableFileSyncNGSC be van állítva, és a 1 értéket adja meg, nyissa meg a kulcsot, és módosítsa az értéket 0-ra.</span><span class="sxs-lookup"><span data-stu-id="446c7-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="446c7-107">A OneDrive manuális elindítása a Start menüben</span><span class="sxs-lookup"><span data-stu-id="446c7-107">Manually launch OneDrive by going to Start</span></span> ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="446c7-109">mezőbe írja be a OneDrive kifejezést, és kattintson az asztali OneDrive alkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="446c7-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="446c7-110">**A OneDrive alaphelyzetbe állítása:**</span><span class="sxs-lookup"><span data-stu-id="446c7-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="446c7-111">Megjegyzi</span><span class="sxs-lookup"><span data-stu-id="446c7-111">Notes:</span></span>

- <span data-ttu-id="446c7-112">A OneDrive alaphelyzetbe állításával az összes meglévő szinkronizálási kapcsolatot leválasztja (a beállítás esetén a személyes OneDrive is).</span><span class="sxs-lookup"><span data-stu-id="446c7-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="446c7-113">A számítógépén a OneDrive alaphelyzetbe állításával nem veszíthet el fájlokat vagy adatot.</span><span class="sxs-lookup"><span data-stu-id="446c7-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="446c7-114">**A OneDrive alaphelyzetbe állítása:**</span><span class="sxs-lookup"><span data-stu-id="446c7-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="446c7-115">Nyisson meg egy Futtatás párbeszédpanelt a Windows billentyű és az R billentyű lenyomásával.</span><span class="sxs-lookup"><span data-stu-id="446c7-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="446c7-116">Írja be a% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset, és nyomja le az OK gombot.</span><span class="sxs-lookup"><span data-stu-id="446c7-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="446c7-117">Előfordulhat, hogy egy parancssorablak is megjelenik röviden.</span><span class="sxs-lookup"><span data-stu-id="446c7-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="446c7-118">A OneDrive manuális elindítása a Start menüben</span><span class="sxs-lookup"><span data-stu-id="446c7-118">Manually launch OneDrive by going to Start</span></span> ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="446c7-120">mezőbe írja be a OneDrive kifejezést, és kattintson az asztali OneDrive alkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="446c7-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="446c7-121">Megjegyzi</span><span class="sxs-lookup"><span data-stu-id="446c7-121">Notes:</span></span>

- <span data-ttu-id="446c7-122">Ha úgy döntött, hogy az Alaphelyzetbe állítás előtt csak bizonyos mappákat szinkronizál, akkor a szinkronizálás befejeződése után ismét el kell végeznie ezt a műveletet.</span><span class="sxs-lookup"><span data-stu-id="446c7-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="446c7-123">További információért olvassa el a [számítógépen szinkronizálandó OneDrive-mappák kiválasztása](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)című témakört   .</span><span class="sxs-lookup"><span data-stu-id="446c7-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="446c7-124">A személyes OneDrive és a OneDrive vállalati verzióhoz ezt el kell végeznie.</span><span class="sxs-lookup"><span data-stu-id="446c7-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>