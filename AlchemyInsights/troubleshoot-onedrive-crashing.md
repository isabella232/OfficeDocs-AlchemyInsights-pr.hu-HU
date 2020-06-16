---
title: A OneDrive összeomlásának elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748921"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6fd57-102">A OneDrive összeomlásának elhárítása</span><span class="sxs-lookup"><span data-stu-id="6fd57-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6fd57-103">Ha a OneDrive ismételten összeomlik, próbálkozzon az alábbi hibaelhárítási lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="6fd57-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6fd57-104">**Győződjön meg arról, hogy a beállításkulcsok nincsenek beállítva:**</span><span class="sxs-lookup"><span data-stu-id="6fd57-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6fd57-105">A Rendszerleíróadatbázis-szerkesztő segítségével keresse meg a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive mappát</span><span class="sxs-lookup"><span data-stu-id="6fd57-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6fd57-106">Ha a DisableFileSyncNGSC jelen van, és értéke 1, nyissa meg a kulcsot, és módosítsa az értéket 0-ra.</span><span class="sxs-lookup"><span data-stu-id="6fd57-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6fd57-107">A OneDrive manuális elindítása a kezdőképernyőn</span><span class="sxs-lookup"><span data-stu-id="6fd57-107">Manually launch OneDrive by going to Start</span></span> ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6fd57-109">, írja be a OneDrive kifejezést a keresőmezőbe, majd kattintson az asztali OneDrive alkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="6fd57-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6fd57-110">**OneDrive alaphelyzetbe állítása:**</span><span class="sxs-lookup"><span data-stu-id="6fd57-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6fd57-111">Megjegyzések:</span><span class="sxs-lookup"><span data-stu-id="6fd57-111">Notes:</span></span>

- <span data-ttu-id="6fd57-112">A OneDrive alaphelyzetbe állításával leválasztja az összes meglévő szinkronizálási kapcsolatot (beleértve a személyes OneDrive-ot is, ha be van állítva).</span><span class="sxs-lookup"><span data-stu-id="6fd57-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6fd57-113">A OneDrive visszaállításával nem veszíti el a fájlokat és az adatokat.</span><span class="sxs-lookup"><span data-stu-id="6fd57-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6fd57-114">**A OneDrive alaphelyzetbe állítása:**</span><span class="sxs-lookup"><span data-stu-id="6fd57-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6fd57-115">A Futtatás párbeszédpanel megnyitása a Windows billentyű és az R billentyű lenyomásával.</span><span class="sxs-lookup"><span data-stu-id="6fd57-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6fd57-116">Írja be a(z) %localappdata%\Microsoft\OneDrive\onedrive.exe /reset parancsot, és nyomja le az OK gombot.</span><span class="sxs-lookup"><span data-stu-id="6fd57-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6fd57-117">Rövid ideig megjelenhet egy parancsablak.</span><span class="sxs-lookup"><span data-stu-id="6fd57-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6fd57-118">A OneDrive manuális elindítása a kezdőképernyőn</span><span class="sxs-lookup"><span data-stu-id="6fd57-118">Manually launch OneDrive by going to Start</span></span> ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6fd57-120">, írja be a OneDrive kifejezést a keresőmezőbe, majd kattintson az asztali OneDrive alkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="6fd57-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6fd57-121">Megjegyzések:</span><span class="sxs-lookup"><span data-stu-id="6fd57-121">Notes:</span></span>

- <span data-ttu-id="6fd57-122">Ha úgy döntött, hogy csak néhány mappát szinkronizál az alaphelyzetbe állítás előtt, akkor ezt újra meg kell tennie, miután a szinkronizálás befejeződött.</span><span class="sxs-lookup"><span data-stu-id="6fd57-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6fd57-123">További [információért válassza ki, hogy mely OneDrive-mappákat szeretné szinkronizálni a](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   számítógéppel.</span><span class="sxs-lookup"><span data-stu-id="6fd57-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6fd57-124">Ezt személyes OneDrive-ja és OneDrive Vállalati verziója esetén is el kell végeznie.</span><span class="sxs-lookup"><span data-stu-id="6fd57-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>