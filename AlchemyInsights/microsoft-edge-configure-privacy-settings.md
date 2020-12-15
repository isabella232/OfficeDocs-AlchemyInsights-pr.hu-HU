---
title: Microsoft Edge – adatvédelmi beállítások megadása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677793"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="d01ae-102">Microsoft Edge – adatvédelmi beállítások megadása</span><span class="sxs-lookup"><span data-stu-id="d01ae-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="d01ae-103">Alapértelmezés szerint, ha a Microsoft Edge nem Windows rendszerű platformokon van telepítve, a diagnosztikai adatok és a webhely adatai nem lesznek elküldve a Microsoftnak.</span><span class="sxs-lookup"><span data-stu-id="d01ae-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="d01ae-104">Ha azonban a Microsoft Edge telepítve van a Windows 10 rendszerben, a diagnosztikai adatokat és a webhely adatait a felhasználók [Windows-diagnosztikai adatbeállításai](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)szerint küldi el a rendszer.</span><span class="sxs-lookup"><span data-stu-id="d01ae-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="d01ae-105">Ha meg szeretné adni, hogy a Microsoft Edge hogyan kezelje a szervezet adatgyűjteményét, használja az alábbi csoportházirend-beállításokat:</span><span class="sxs-lookup"><span data-stu-id="d01ae-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="d01ae-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ez a házirend lehetővé teszi a használat és az összeomlással kapcsolatos adatok jelentését.</span><span class="sxs-lookup"><span data-stu-id="d01ae-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="d01ae-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ez a házirend a Microsoft Services fejlesztéséhez használt webhely-információkat küldi.</span><span class="sxs-lookup"><span data-stu-id="d01ae-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="d01ae-108">További információt a házirend- [beállítások megadása](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="d01ae-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>