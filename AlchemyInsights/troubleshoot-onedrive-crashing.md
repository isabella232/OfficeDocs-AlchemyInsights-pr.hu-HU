---
title: A OneDrive összeomlásának elhárítása
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826201"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="a8ecf-102">A OneDrive összeomlásának elhárítása</span><span class="sxs-lookup"><span data-stu-id="a8ecf-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="a8ecf-103">Ha a OneDrive ismétlődően összeomlik, próbálkozzon az alábbi hibaelhárítási lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="a8ecf-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="a8ecf-104">**Győződjön meg arról, hogy nincsenek beállítva beállításkulcsok:**</span><span class="sxs-lookup"><span data-stu-id="a8ecf-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="a8ecf-105">A Beállításszerkesztővel lépjen a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="a8ecf-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="a8ecf-106">Ha a DisableFileSyncNGSC 1 értékre van állítva, nyissa meg a kulcsot, és módosítsa az értéket 0-ra.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="a8ecf-107">Indítsa el manuálisan a OneDrive-ot a Start menüben</span><span class="sxs-lookup"><span data-stu-id="a8ecf-107">Manually launch OneDrive by going to Start</span></span> ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a8ecf-109">, írja be a OneDrive keresőt a keresőmezőbe, majd kattintson az asztali OneDrive appra.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a8ecf-110">**A OneDrive alaphelyzetbe állítása:**</span><span class="sxs-lookup"><span data-stu-id="a8ecf-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="a8ecf-111">Megjegyzések:</span><span class="sxs-lookup"><span data-stu-id="a8ecf-111">Notes:</span></span>

- <span data-ttu-id="a8ecf-112">A OneDrive alaphelyzetbe állításával az összes meglévő szinkronizálási kapcsolatot leválasztja (beleértve a személyes OneDrive-ot is, ha be van állítva).</span><span class="sxs-lookup"><span data-stu-id="a8ecf-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="a8ecf-113">A OneDrive számítógépen való alaphelyzetbe állításával nem veszít el fájlokat vagy adatokat.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="a8ecf-114">**A OneDrive alaphelyzetbe állítása:**</span><span class="sxs-lookup"><span data-stu-id="a8ecf-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="a8ecf-115">Nyisson meg egy Futtatás párbeszédpanelt a Windows billentyű és az R billentyű lenyomásával.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="a8ecf-116">Írja be a %localappdata%\Microsoft\OneDrive\onedrive.exe /reset parancsot, és nyomja le az OK gombot.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="a8ecf-117">A parancsablak röviden megjelenhet.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="a8ecf-118">Indítsa el manuálisan a OneDrive-ot a Start menüben</span><span class="sxs-lookup"><span data-stu-id="a8ecf-118">Manually launch OneDrive by going to Start</span></span> ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a8ecf-120">, írja be a OneDrive keresőt a keresőmezőbe, majd kattintson az asztali OneDrive appra.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a8ecf-121">Megjegyzések:</span><span class="sxs-lookup"><span data-stu-id="a8ecf-121">Notes:</span></span>

- <span data-ttu-id="a8ecf-122">Ha úgy döntött, hogy csak bizonyos mappákat szinkronizál az alaphelyzetbe állítás előtt, azt a szinkronizálás befejezése után ismét el kell indítania.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="a8ecf-123">További információ: A [számítógépre szinkronizálni kívánt OneDrive-mappák](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   kiválasztása.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="a8ecf-124">Ezt személyes OneDrive- és OneDrive Vállalati verziós tárterülete esetén kell végrehajtania.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>