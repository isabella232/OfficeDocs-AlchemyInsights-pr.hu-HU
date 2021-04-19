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
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="3dbcd-102">A portálon hiányzó Konfigurációkezelőbeli eszközök</span><span class="sxs-lookup"><span data-stu-id="3dbcd-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="3dbcd-103">Az eszközszinkronizálás működéséhez [szükséges internetes végpontoknak](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) elérhetőknek kell lenniük a szolgáltatás csatlakozási pontjának szerepkörét futtató helyszíni kiszolgálóról.</span><span class="sxs-lookup"><span data-stu-id="3dbcd-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="3dbcd-104">Az eszközszinkronizálással kapcsolatos hibaelhárításhoz tekintse át a szolgáltatás kapcsolódási pontján található **CMGatewaySyncUploadWorker.log** fájlt.</span><span class="sxs-lookup"><span data-stu-id="3dbcd-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="3dbcd-105">Bővebben olvashat arról, hogyan [csatlakoztathat bérlőt a Microsoft Endpoint Managerben](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="3dbcd-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
