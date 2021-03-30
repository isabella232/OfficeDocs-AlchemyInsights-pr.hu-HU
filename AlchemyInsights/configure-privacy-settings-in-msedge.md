---
title: Adatvédelmi beállítások megadása a Microsoft Edge-ben
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405106"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="a3c75-102">Adatvédelmi beállítások megadása a Microsoft Edge-ben</span><span class="sxs-lookup"><span data-stu-id="a3c75-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="a3c75-103">Alapértelmezés szerint, ha a Microsoft Edge nem Windows-platformokon van telepítve, a diagnosztikai adatokat és a webhelyadatokat a rendszer nem küldi el a Microsoftnak.</span><span class="sxs-lookup"><span data-stu-id="a3c75-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="a3c75-104">Ha azonban a Microsoft Edge a Windows 10-ben van telepítve, a diagnosztikai adatokat és a webhelyadatokat a felhasználók Windows diagnosztikai adataira [vonatkozó beállításai alapján küldi el a rendszer.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="a3c75-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="a3c75-105">Az alábbi csoportházirendekkel konfigurálhatja, hogy a Microsoft Edge hogyan kezelje az adatgyűjtést a szervezetében:</span><span class="sxs-lookup"><span data-stu-id="a3c75-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="a3c75-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) – Bekapcsolja a használattal és az összeomlással kapcsolatos adatok jelentését.</span><span class="sxs-lookup"><span data-stu-id="a3c75-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="a3c75-107">[A SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) elküldi a Microsoft-szolgáltatások javítására használt webhelyadatokat.</span><span class="sxs-lookup"><span data-stu-id="a3c75-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="a3c75-108">További információ: [Házirend-beállítások konfigurálása.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="a3c75-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
