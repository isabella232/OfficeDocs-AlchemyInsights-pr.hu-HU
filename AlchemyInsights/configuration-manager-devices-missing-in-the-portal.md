---
title: A portálon hiányzó Konfigurációkezelőbeli eszközök
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789904"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>A portálon hiányzó Konfigurációkezelőbeli eszközök

Az eszközszinkronizálás működéséhez [szükséges internetes végpontoknak](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) elérhetőknek kell lenniük a szolgáltatás csatlakozási pontjának szerepkörét futtató helyszíni kiszolgálóról. Az eszközszinkronizálással kapcsolatos hibaelhárításhoz tekintse át a szolgáltatás kapcsolódási pontján található **CMGatewaySyncUploadWorker.log** fájlt.

Bővebben olvashat arról, hogyan [csatlakoztathat bérlőt a Microsoft Endpoint Managerben](https://docs.microsoft.com/configmgr/tenant-attach/).
