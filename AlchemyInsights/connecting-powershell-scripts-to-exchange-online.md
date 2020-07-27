---
title: PowerShell-parancsfájlok csatlakoztatása az Exchange Online-hoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 34301e62a25e11c5d4c353166f8208ef74245dfa
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423512"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="93247-102">PowerShell-parancsfájlok csatlakoztatása az Exchange Online-hoz</span><span class="sxs-lookup"><span data-stu-id="93247-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="93247-103">Az Exchange Online alapfokú hitelesítése elavult lesz, és az előrevezető út a parancsfájlok és a felügyelet nélküli feladatok tanúsítványalapú hitelesítésével történő csatlakozás.</span><span class="sxs-lookup"><span data-stu-id="93247-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="93247-104">További információt az [EXO V2 modul felügyelet nélküli parancsfájljainak csak alkalmazáshitelesítése című témakörben olvashat.](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2)</span><span class="sxs-lookup"><span data-stu-id="93247-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>