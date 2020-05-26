---
title: A Windows memóriadiagnosztika futtatása a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357791"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="53ace-102">A Windows memóriadiagnosztika futtatása a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="53ace-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="53ace-103">Ha a Windows és a számítógépen lévő alkalmazások összeomlanak, lefagynak vagy instabil módon működnek, akkor lehet, hogy probléma van a számítógép memóriájával (RAM).</span><span class="sxs-lookup"><span data-stu-id="53ace-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="53ace-104">A Windows memóriadiagnosztika futtatásával ellenőrizheti, hogy vannak-e problémák a számítógép RAM memóriájával kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="53ace-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="53ace-105">A tálca keresőmezőjébe írja be a **memóriadiagnosztika parancsot,** majd válassza a **Windows memóriadiagnosztika**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="53ace-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="53ace-106">A diagnosztika futtatásához a számítógépnek újra kell indulnia.</span><span class="sxs-lookup"><span data-stu-id="53ace-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="53ace-107">Lehetősége van arra, hogy azonnal újrainduljon (mentse el a munkáját, és először zárja be a megnyitott dokumentumokat és e-maileket), vagy ütemezze a diagnosztikát úgy, hogy automatikusan fusson a számítógép következő újraindításakor:</span><span class="sxs-lookup"><span data-stu-id="53ace-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows memóriadiagnosztika](media/windows-memory-diagnostic.png)

<span data-ttu-id="53ace-109">Amikor a számítógép újraindul, a **Windows memóriadiagnosztikai eszköz** automatikusan elindul.</span><span class="sxs-lookup"><span data-stu-id="53ace-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="53ace-110">Az állapot és a folyamat a diagnosztika futása közben jelenik meg, és lehetősége van a diagnosztika megszakítására az **ESC** billentyű nek a billentyűzeten való megnyomásával.</span><span class="sxs-lookup"><span data-stu-id="53ace-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="53ace-111">Amikor a diagnosztika befejeződött, a Windows a szokásos módon indul el.</span><span class="sxs-lookup"><span data-stu-id="53ace-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="53ace-112">Közvetlenül az újraindítás után, amikor az asztal megjelenik, egy értesítés jelenik meg (a **műveletközpont** ikonja mellett a tálcán), jelezve, hogy találtak-e memóriahibákat.</span><span class="sxs-lookup"><span data-stu-id="53ace-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="53ace-113">Például:</span><span class="sxs-lookup"><span data-stu-id="53ace-113">For example:</span></span>

<span data-ttu-id="53ace-114">A Műveletközpont ikonja:</span><span class="sxs-lookup"><span data-stu-id="53ace-114">Here's the Action Center icon:</span></span> ![A Műveletközpont ikonja](media/action-center-icon.png) 

<span data-ttu-id="53ace-116">És egy minta értesítés:</span><span class="sxs-lookup"><span data-stu-id="53ace-116">And a sample notification:</span></span> ![Nincsmemória-hiba](media/no-memory-errors.png)

<span data-ttu-id="53ace-118">Ha nem fogadott el az értesítést, a **műveletközpont** ikonja a tálcán a **Műveletközpont** megjelenítéséhez és az értesítések görgethető listájának megjelenítéséhez.</span><span class="sxs-lookup"><span data-stu-id="53ace-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="53ace-119">A részletes információk áttekintéséhez írja be az **eseményt** a tálca keresőmezőjébe, és válassza az **Eseménynapló**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="53ace-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="53ace-120">Az **Eseménynapló**bal oldali ablaktáblájában keresse meg a **Windows naplók > System ablakot.**</span><span class="sxs-lookup"><span data-stu-id="53ace-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="53ace-121">A jobb oldali ablaktáblában olvassa be a listát, miközben a **Forrás** oszlopot nézi, amíg meg nem jelennek a **MemoryDiagnostics-Results**forrásértékű események.</span><span class="sxs-lookup"><span data-stu-id="53ace-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="53ace-122">Jelölje ki az egyes eseményeket, és tekintse meg az eredményadatokat a lista alatti **Általános** lap alatt található mezőben.</span><span class="sxs-lookup"><span data-stu-id="53ace-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
