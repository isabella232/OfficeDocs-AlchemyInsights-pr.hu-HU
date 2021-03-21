---
title: Problémák akkor, amikor gépeket vezet be a Végponthoz készült Microsoft Defenderhez (MDE)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901569"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="d2f75-102">Problémák akkor, amikor gépeket vezet be a Végponthoz készült Microsoft Defenderhez (MDE)</span><span class="sxs-lookup"><span data-stu-id="d2f75-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="d2f75-103">Problémákat észlelhet akkor, amikor gépeket próbál bevezetni az MDE szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="d2f75-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="d2f75-104">Ha hozzá tud férni a végfelhasználói géphez, kövesse ezeket a lépéseket:</span><span class="sxs-lookup"><span data-stu-id="d2f75-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="d2f75-105">A [MDE Klienselemző](https://aka.ms/betamdeanalyzer) diagnosztikai eszköz legújabb előzetes verziójának letöltése.</span><span class="sxs-lookup"><span data-stu-id="d2f75-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="d2f75-106">Kattintson jobb kattintással a **MDEClientAnalyzer.cmd** elemre, és válassza a „Futtatás rendszergazdaként“ lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d2f75-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="d2f75-107">Kövesse a javasolt utasításokat a **MDEClientAnalyzer.htm** elemben megadottak szerint.</span><span class="sxs-lookup"><span data-stu-id="d2f75-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="d2f75-108">Részletesebb naplókért tekintse át a létrehozott almappát:**MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="d2f75-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="d2f75-109">Ha további útmutatásra van szüksége, lépjen kapcsolatba a [Végponthoz készült Microsoft Defender támogatással](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) és adja meg a létrehozott MDEClientAnalyzerResult.zip fájlt elemzésre.</span><span class="sxs-lookup"><span data-stu-id="d2f75-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
