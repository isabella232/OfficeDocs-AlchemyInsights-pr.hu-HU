---
title: Nem sikerül dupla kattintással megnyitni egy Office-fájlt
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814807"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="c3134-102">Nem sikerül dupla kattintással megnyitni egy Office-fájlt</span><span class="sxs-lookup"><span data-stu-id="c3134-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="c3134-103">Miután duplán kattintott egy Office-fájlra, előfordulhat, hogy a program megnyílik, de maga a fájl nem nyílik meg.</span><span class="sxs-lookup"><span data-stu-id="c3134-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="c3134-104">Vagy a következő hibaüzenet jelenhet meg: "Nem sikerült elküldeni a parancsot a programnak".</span><span class="sxs-lookup"><span data-stu-id="c3134-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="c3134-105">Ennek számos oka lehet, de a két leggyakoribb megoldás:</span><span class="sxs-lookup"><span data-stu-id="c3134-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="c3134-106">Az Excelben győződjön meg arról, hogy a DDE beállítás nincs bejelölve.</span><span class="sxs-lookup"><span data-stu-id="c3134-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="c3134-107">Ez a lehetőség úgy található meg, hogy létrehoz egy új munkafüzetet, majd a Fájlbeállítások **> Beállítások > gombra.**</span><span class="sxs-lookup"><span data-stu-id="c3134-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="c3134-108">Az Általános **csoportban** törölje a jelölést a **DDE (Dynamic Data Exchange)**(Egyéb alkalmazások mellőzása) jelölőnégyzetből.</span><span class="sxs-lookup"><span data-stu-id="c3134-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="c3134-109">Az alapértelmezett beállítások visszaállításához futtasson online javítást.</span><span class="sxs-lookup"><span data-stu-id="c3134-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="c3134-110">Kattintson a Windows Start gombjára, és keressen rá a "Vezérlőpult" kifejezésre.</span><span class="sxs-lookup"><span data-stu-id="c3134-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="c3134-111">Nyissa meg **a Vezérlőpultot,** majd a **Programok és szolgáltatások > gombra.**</span><span class="sxs-lookup"><span data-stu-id="c3134-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="c3134-112">Ezután kattintson a jobb gombbal a **Microsoft Office [Verzió]** elemre, és válassza **az Online > lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c3134-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="c3134-113">Ha egyik megoldás sem működik, a támogatási cikkben talál egy teljesebb megoldáslistát, ha egy [Office-fájlra](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)duplán kattintva nem nyílik meg.</span><span class="sxs-lookup"><span data-stu-id="c3134-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
