---
title: Meghajtószállítás az Microsoft 365 importálási szolgáltatásban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731650"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="9e4e9-102">Meghajtószállítás az Microsoft 365 importálási szolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="9e4e9-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="9e4e9-103">A Meghajtószállítást úgy használhatja, hogy PST-fájlokat másol egy merevlemezre, majd a merevlemezt a Microsoftnak szállítja.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="9e4e9-104">A feladat elkezdeni:</span><span class="sxs-lookup"><span data-stu-id="9e4e9-104">To start the job:</span></span>

1. <span data-ttu-id="9e4e9-105">Az Microsoft 365 Megfelelőségi központban az **Információirányítás alatt válassza** az **Importálás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9e4e9-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="9e4e9-106">Válassza **az Importálási feladattípus kiválasztása lehetőséget,** majd a Tovább **gombot.**</span><span class="sxs-lookup"><span data-stu-id="9e4e9-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="9e4e9-107">Az importálási beállítás lépéseit a Merevlemezek egyikének szállítja a fizikai helyek egyikének a **gombra választva láthatja.**</span><span class="sxs-lookup"><span data-stu-id="9e4e9-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="9e4e9-108">Néhány dolog, amit meg kell emlékeznie:</span><span class="sxs-lookup"><span data-stu-id="9e4e9-108">Here are some things to remember:</span></span>

- <span data-ttu-id="9e4e9-109">A PST-fájlok postaládákba való importálásának Exchange Online postaláda-importálási Microsoft 365 kell.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="9e4e9-110">A 20 GB-ot nagyobb PST-fájlok teljesítménye is befolyásolhatja.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="9e4e9-111">Csak a 2,5 hüvelykes SSD-meghajtók, illetve a 2,5 vagy 3,5 hüvelykes SATA II/III típusú belső merevlemezek támogatottak.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="9e4e9-112">A PST-fájlokat tartalmazó merevlemezt titkosítva kell BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="9e4e9-113">A PST-fájlok meghajtószállítással történő Microsoft 365 a PST-fájlok importálásának költsége GB-onként 2 USD.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="9e4e9-114">A Meghajtószállítási módszer PST-fájlok importálásával kapcsolatos további információkért lásd: A szervezet PST-fájljainak importálása meghajtószállítás [használatával.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="9e4e9-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>