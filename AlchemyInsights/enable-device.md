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
# <a name="enable-device"></a>Eszköz engedélyezése

**Az eszköz engedélyezése a PowerShell parancs használatával**

Futtassa a következő parancsokat:

- Eszközobjektum lekérte: `Get-MsolDevice -Name <Name>`
- Eszköz engedélyezése: `Enable-MsolDevice -DeviceId <DeviceId>`

A Hibrid csatlakozás felügyelt tartományokon való konfigurálásával kapcsolatos további információkért lásd: Hibrid csatlakozás [konfigurálása.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
