---
title: A Microsoft Edge telepítése, frissítése és kezelése a Konfigurációkezelő segítségével a Windowsban
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004030"
- "7100"
ms.openlocfilehash: 8987a37a1e756001c45e9407337543d70560e314
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677870"
---
# <a name="use-configuration-manager-to-deploy-update-and-manage-microsoft-edge-on-windows"></a><span data-ttu-id="e818a-102">A Microsoft Edge telepítése, frissítése és kezelése a Konfigurációkezelő segítségével a Windowsban</span><span class="sxs-lookup"><span data-stu-id="e818a-102">Use Configuration Manager to deploy, update, and manage Microsoft Edge on Windows</span></span>

<span data-ttu-id="e818a-103">A Configuration Manager 1910-es verziójának használatával a Microsoft Edge (77-es vagy újabb verzió) telepíthető PowerShell-parancsfájlon keresztül.</span><span class="sxs-lookup"><span data-stu-id="e818a-103">As of Configuration Manager version 1910, you can deploy Microsoft Edge (versions 77 and later) through a PowerShell script.</span></span> <span data-ttu-id="e818a-104">A parancsfájl kikapcsolja az automatikus frissítéseket, így így kezelheti a frissítéseket a Configuration Manager segítségével.</span><span class="sxs-lookup"><span data-stu-id="e818a-104">The script turns off automatic updates, and this lets you manage the updates through Configuration Manager.</span></span> <span data-ttu-id="e818a-105">Ha többet szeretne tudni a Konfigurációkezelő használatáról és egyéb előnyeiről, olvassa el a [Microsoft Edge Management](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge?)című témakört.</span><span class="sxs-lookup"><span data-stu-id="e818a-105">To learn more about this and other benefits of using Configuration Manager, see [Microsoft Edge Management](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge?).</span></span>