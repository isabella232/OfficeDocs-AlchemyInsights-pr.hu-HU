---
title: A Windows memóriadiagnosztika futtatása a Windows 10-ben
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826669"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="cbb9d-102">A Windows memóriadiagnosztika futtatása a Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="cbb9d-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="cbb9d-103">Ha a Windows és a PC-n telepített alkalmazások összeomlanak, lefagynak vagy instabilan működnek, probléma lehet a PC memóriájával (a RAM-mal).</span><span class="sxs-lookup"><span data-stu-id="cbb9d-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="cbb9d-104">A Windows memóriadiagnosztika futtatásával ellenőrizheti, hogy vannak-e problémák a PC RAM-jával kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="cbb9d-105">A tálcán lévő keresőmezőbe írja be a **memóriadiagnosztika** szót, majd válassza ki a **Windows memóriadiagnosztika** alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="cbb9d-106">A diagnosztika futtatásához a PC-nek újra kell indulnia.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="cbb9d-107">Lehetősége van azonnal újraindítani a PC-t (először mentse a munkáját, és zárja be a megnyitott dokumentumokat és e-maileket), vagy beütemezheti a diagnosztika automatikus futtatását a PC következő újraindulásakor:</span><span class="sxs-lookup"><span data-stu-id="cbb9d-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows memóriadiagnosztika](media/windows-memory-diagnostic.png)

<span data-ttu-id="cbb9d-109">A PC újraindítása után automatikusan futni kezd a **Windows memóriadiagnosztika eszköz**.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="cbb9d-110">A diagnosztika futása során megjelenik az állapot és a folyamat előrehaladása, és a billentyűzeten levő **ESC** billentyű lenyomásával megszakíthatja a diagnosztikát.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="cbb9d-111">A diagnosztika befejeződése után a Windows a szokásos módon elindul.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="cbb9d-112">Közvetlenül az újraindítás után, az asztal megjelenésekor megjelenik egy értesítés (a tálcán lévő **Műveletközpont** ikon mellett), amely jelzi, hogy találhatók-e memóriahibák.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="cbb9d-113">Például:</span><span class="sxs-lookup"><span data-stu-id="cbb9d-113">For example:</span></span>

<span data-ttu-id="cbb9d-114">Ez itt a Műveletközpont ikonja:</span><span class="sxs-lookup"><span data-stu-id="cbb9d-114">Here's the Action Center icon:</span></span> ![Műveletközpont ikon](media/action-center-icon.png) 

<span data-ttu-id="cbb9d-116">Ez pedig egy példa az értesítésre:</span><span class="sxs-lookup"><span data-stu-id="cbb9d-116">And a sample notification:</span></span> ![Nincs memóriahiba](media/no-memory-errors.png)

<span data-ttu-id="cbb9d-118">Ha elmulasztotta az értesítést, a tálcán lévő **Műveletközpont** ikon kiválasztásával megjelenítheti a **Műveletközpontot**, amely tartalmazza az értesítések görgethető listáját.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="cbb9d-119">A részletes információk áttekintéséhez írja be az **esemény** szót a tálcán található keresőmezőbe, majd válassza az **Eseménynapló** alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="cbb9d-120">Az **Eseménynapló** bal oldali ablaktáblájában lépjen a **Windows-naplók > Rendszer** elemre.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="cbb9d-121">A jobb oldali ablaktáblában fentről lefelé haladva nézze át a listát, és figyelje a **Forrás** oszlopot, amíg nem talál olyan eseményeket, amelyeknél a Forrás értéke **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="cbb9d-122">Jelölje ki sorban mindegyik ilyen eseményt, és a lista alatti **Általános** lapon levő mezőben tekintse meg az eredményeket.</span><span class="sxs-lookup"><span data-stu-id="cbb9d-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
