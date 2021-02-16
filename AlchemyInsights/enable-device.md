---
title: Eszköz engedélyezése
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256870"
---
# <a name="enable-device"></a><span data-ttu-id="6facc-102">Eszköz engedélyezése</span><span class="sxs-lookup"><span data-stu-id="6facc-102">Enable Device</span></span>

<span data-ttu-id="6facc-103">**Az eszköz engedélyezése a PowerShell parancs használatával**</span><span class="sxs-lookup"><span data-stu-id="6facc-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="6facc-104">Futtassa a következő parancsokat:</span><span class="sxs-lookup"><span data-stu-id="6facc-104">Run the following commands:</span></span>

- <span data-ttu-id="6facc-105">Eszközobjektum lekérte: `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="6facc-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="6facc-106">Eszköz engedélyezése: `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="6facc-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="6facc-107">A Hibrid csatlakozás felügyelt tartományokon való konfigurálásával kapcsolatos további információkért lásd: Hibrid csatlakozás [konfigurálása.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)</span><span class="sxs-lookup"><span data-stu-id="6facc-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
