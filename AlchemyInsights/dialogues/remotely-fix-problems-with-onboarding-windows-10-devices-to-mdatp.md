---
title: A Windows 10-es eszközök Microsoft Defender komplex veszélyforrások elleni védelme szolgáltatásba való be- és beállításával kapcsolatos problémák távoli megoldása
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693654"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="930d2-102">A Windows 10-es eszközök Microsoft Defender komplex veszélyforrások elleni védelme szolgáltatásba való be- és beállításával kapcsolatos problémák távoli megoldása</span><span class="sxs-lookup"><span data-stu-id="930d2-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="930d2-103">Ha hozzá tud férni a távoli számítógéphez, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="930d2-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="930d2-104">Töltse le [az Ügyfélkapcsolat-elemző diagnosztikai](https://go.microsoft.com/fwlink/?linkid=2143466) eszközt.</span><span class="sxs-lookup"><span data-stu-id="930d2-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="930d2-105">Az MDATPAnalyzer.cmd kinyerása és futtatása.</span><span class="sxs-lookup"><span data-stu-id="930d2-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="930d2-106">Keresse meg a diagnosztikai naplót az MDATPClientAnalyzerResult mappában, amely ugyanaz a mappa, amelybe az elemző eszközt letöltötte.</span><span class="sxs-lookup"><span data-stu-id="930d2-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="930d2-107">Ha csatlakozási vagy internetes proxybeállításokkal kapcsolatos problémákat keres, tekintse át a naplófájlt MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="930d2-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="930d2-108">További információt a berakható gépekkel [kapcsolatos problémákban olvashat.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="930d2-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
