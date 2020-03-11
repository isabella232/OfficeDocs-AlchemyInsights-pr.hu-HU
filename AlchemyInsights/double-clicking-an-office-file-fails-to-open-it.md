---
title: Ha duplán kattint egy Office-fájlra, nem nyitja meg
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573525"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="e4c63-102">Ha duplán kattint egy Office-fájlra, nem nyitja meg</span><span class="sxs-lookup"><span data-stu-id="e4c63-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="e4c63-103">Miután duplán kattintott egy Office-fájlra, előfordulhat, hogy a program megnyílik, de maga a fájl nem nyílik meg.</span><span class="sxs-lookup"><span data-stu-id="e4c63-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="e4c63-104">Vagy lehet, hogy a hiba: "Volt egy probléma elküldi a parancsot a program."</span><span class="sxs-lookup"><span data-stu-id="e4c63-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="e4c63-105">Ennek számos oka van, de a két leggyakoribb megoldás a következő:</span><span class="sxs-lookup"><span data-stu-id="e4c63-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="e4c63-106">Az Excelből győződjön meg arról, hogy a DDE beállítás nincs bejelölve.</span><span class="sxs-lookup"><span data-stu-id="e4c63-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="e4c63-107">A beállítás megtalálható egy új munkafüzet létrehozásával, majd a **Fájl > beállítások > Speciális**parancs kiválasztásával.</span><span class="sxs-lookup"><span data-stu-id="e4c63-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="e4c63-108">Az **Általános** szakaszban törölje a jelet a **Dinamikus adatcserét (DDE) használó egyéb alkalmazások figyelmen kívül hagyása jelölőnégyzetből.**</span><span class="sxs-lookup"><span data-stu-id="e4c63-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="e4c63-109">Az alapértelmezett beállítások visszaállításához futtasson online javítást.</span><span class="sxs-lookup"><span data-stu-id="e4c63-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="e4c63-110">Kattintson a Windows Start gombjára, és keressen a "Vezérlőpult" kifejezésre.</span><span class="sxs-lookup"><span data-stu-id="e4c63-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="e4c63-111">Nyissa meg a **Vezérlőpultot,** és nyissa meg a Programok > Programok és szolgáltatások című **lapot.**</span><span class="sxs-lookup"><span data-stu-id="e4c63-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="e4c63-112">Ezután kattintson a jobb gombbal a **Microsoft Office [Version]** elemre, és válassza **> Online javítás módosítása parancsot.**</span><span class="sxs-lookup"><span data-stu-id="e4c63-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="e4c63-113">Ha egyik megoldás sem működik, a támogatási cikkben található a megoldások teljesebb listája, az [Office-fájlokra duplán kattintva nem nyithatja meg.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="e4c63-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
