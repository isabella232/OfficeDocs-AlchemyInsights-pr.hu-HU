---
title: A Windows Virtual Desktop-hoz tartozó munkamenetgazda-képek testreszabása
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
- "9003902"
- "6957"
ms.openlocfilehash: 23bf130aad5bafa6756f0adfc2e58a130c2f6c4e
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692057"
---
# <a name="customize-a-session-host-image-for-windows-virtual-desktop"></a><span data-ttu-id="d8aa6-102">A Windows Virtual Desktop-hoz tartozó munkamenetgazda-képek testreszabása</span><span class="sxs-lookup"><span data-stu-id="d8aa6-102">Customize a session host image for Windows Virtual Desktop</span></span>

<span data-ttu-id="d8aa6-103">A virtuális gépek (VM-EK) kétféle módon készíthetők elő a Windows virtuális asztali verziójának fő virtuális merevlemezén:</span><span class="sxs-lookup"><span data-stu-id="d8aa6-103">There are two ways to prepare a virtual machine (VM) by using a master Virtual Hard Disk image for Windows Virtual Desktop:</span></span>

1. <span data-ttu-id="d8aa6-104">[Hozzon létre egy VM-et egy felügyelt képből az Azure-ban](https://go.microsoft.com/fwlink/?linkid=2127906), majd ugorjon a [szoftver előkészítése és telepítése](https://go.microsoft.com/fwlink/?linkid=2128064)előtt.</span><span class="sxs-lookup"><span data-stu-id="d8aa6-104">[Create a VM from a managed image in Azure](https://go.microsoft.com/fwlink/?linkid=2127906), and then skip ahead to the [preparation and installation of software](https://go.microsoft.com/fwlink/?linkid=2128064).</span></span>
1. <span data-ttu-id="d8aa6-105">A képet úgy [hozhatja létre helyileg](https://go.microsoft.com/fwlink/?linkid=2128065) , hogy letölti a képet, [kiépíti a Hyper-V VM-](https://go.microsoft.com/fwlink/?linkid=2127907)et, majd testre szabhatja az igényeinek megfelelően.</span><span class="sxs-lookup"><span data-stu-id="d8aa6-105">[Create the image locally](https://go.microsoft.com/fwlink/?linkid=2128065) by downloading the image, [provisioning a Hyper-V VM](https://go.microsoft.com/fwlink/?linkid=2127907), and then customizing it to suit your needs.</span></span>

<span data-ttu-id="d8aa6-106">További információ: [a fő VHD-Kép előkészítése és testreszabása](https://go.microsoft.com/fwlink/?linkid=2127838).</span><span class="sxs-lookup"><span data-stu-id="d8aa6-106">To learn more, see [Prepare and customize a master VHD image](https://go.microsoft.com/fwlink/?linkid=2127838).</span></span>