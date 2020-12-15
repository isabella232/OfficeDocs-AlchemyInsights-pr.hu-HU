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
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge – adatvédelmi beállítások megadása

Alapértelmezés szerint, ha a Microsoft Edge nem Windows rendszerű platformokon van telepítve, a diagnosztikai adatok és a webhely adatai nem lesznek elküldve a Microsoftnak. Ha azonban a Microsoft Edge telepítve van a Windows 10 rendszerben, a diagnosztikai adatokat és a webhely adatait a felhasználók [Windows-diagnosztikai adatbeállításai](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)szerint küldi el a rendszer.

Ha meg szeretné adni, hogy a Microsoft Edge hogyan kezelje a szervezet adatgyűjteményét, használja az alábbi csoportházirend-beállításokat:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ez a házirend lehetővé teszi a használat és az összeomlással kapcsolatos adatok jelentését.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ez a házirend a Microsoft Services fejlesztéséhez használt webhely-információkat küldi.

További információt a házirend- [beállítások megadása](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)című témakörben találhat.