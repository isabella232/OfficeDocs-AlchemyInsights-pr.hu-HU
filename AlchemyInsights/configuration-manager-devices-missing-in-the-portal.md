---
title: A portálon hiányzó Konfigurációkezelőbeli eszközök
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
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817246"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>A portálon hiányzó Konfigurációkezelőbeli eszközök

Az eszközszinkronizálás működéséhez [szükséges internetes végpontoknak](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) elérhetőknek kell lenniük a szolgáltatás csatlakozási pontjának szerepkörét futtató helyszíni kiszolgálóról. Az eszközszinkronizálással kapcsolatos hibaelhárításhoz tekintse át a szolgáltatás kapcsolódási pontján található **CMGatewaySyncUploadWorker.log** fájlt.

Bővebben olvashat arról, hogyan [csatlakoztathat bérlőt a Microsoft Endpoint Managerben](https://docs.microsoft.com/configmgr/tenant-attach/).
