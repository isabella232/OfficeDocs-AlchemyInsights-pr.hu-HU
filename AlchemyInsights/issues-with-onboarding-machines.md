---
title: A bevezetési gépekkel kapcsolatos problémák
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141469"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="876fb-102">A bevezetési gépekkel kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="876fb-102">Issues with onboarding machines</span></span>

<span data-ttu-id="876fb-103">Lehet, hogy problémák vannak a mdatp-szolgáltatásra való bevezetési gépekkel.</span><span class="sxs-lookup"><span data-stu-id="876fb-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="876fb-104">Ha hozzá tud férni a végfelhasználói számítógéphez, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="876fb-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="876fb-105">Töltse le az [Ügyfélkapcsolat-elemző](https://aka.ms/mdatpanalyzer) diagnosztikai eszközt.</span><span class="sxs-lookup"><span data-stu-id="876fb-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="876fb-106">Kivonat és fuss MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="876fb-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="876fb-107">Keresse meg a diagnosztikai naplót az MDATPClientAnalyzerResult nevű mappában, ugyanabban a mappában, ahol az Analyzer eszközt letölti.</span><span class="sxs-lookup"><span data-stu-id="876fb-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="876fb-108">Tekintse át a naplófájlt, MDATPClientAnalyzer.txt, hogy megtalálja a kapcsolódási vagy internetproxy-beállításokkal kapcsolatos problémákat.</span><span class="sxs-lookup"><span data-stu-id="876fb-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>