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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966111"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>A portálon hiányzó Konfigurációkezelőbeli eszközök

Az eszközszinkronizálás működéséhez [szükséges internetes végpontoknak](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) elérhetőknek kell lenniük a szolgáltatás csatlakozási pontjának szerepkörét futtató helyszíni kiszolgálóról. Az eszközszinkronizálással kapcsolatos hibaelhárításhoz tekintse át a szolgáltatás kapcsolódási pontján található **CMGatewaySyncUploadWorker.log** fájlt.

Bővebben olvashat arról, hogyan [csatlakoztathat bérlőt a Microsoft Endpoint Managerben](https://docs.microsoft.com/configmgr/tenant-attach/).
