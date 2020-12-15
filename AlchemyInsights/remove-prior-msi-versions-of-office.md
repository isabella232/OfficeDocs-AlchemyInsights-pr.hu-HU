---
title: Az Office korábbi MSI-verzióinak eltávolítása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680724"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="69c49-102">Az Office korábbi MSI-verzióinak eltávolítása</span><span class="sxs-lookup"><span data-stu-id="69c49-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="69c49-103">Azt javasoljuk, hogy távolítsa el az Office korábbi Windows Installer (MSI) verzióit az Office 365 ProPlus telepítése előtt.</span><span class="sxs-lookup"><span data-stu-id="69c49-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="69c49-104">Ezt a következőképpen teheti meg:</span><span class="sxs-lookup"><span data-stu-id="69c49-104">Here's how to do this:</span></span>

1. <span data-ttu-id="69c49-105">Ha az MSI-t használta az Office telepítéséhez, az Office-telepítő eszköz (ODT) segítségével távolítsa el az Office-t.</span><span class="sxs-lookup"><span data-stu-id="69c49-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="69c49-106">Használhatja a RemoveMSI elemet a **configuration.xml** -fájlban.</span><span class="sxs-lookup"><span data-stu-id="69c49-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="69c49-107">Kövesse a jelen cikk útmutatását: az [Office 365 biztonsági & megfelelőségi központ.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="69c49-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>