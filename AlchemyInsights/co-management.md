---
title: Társ-menedzsment
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910316"
---
# <a name="co-management"></a><span data-ttu-id="7964a-102">Társ-menedzsment</span><span class="sxs-lookup"><span data-stu-id="7964a-102">Co-management</span></span>

<span data-ttu-id="7964a-103">**Előfeltételek a config Manager hibrid és Intune közötti áttelepítéséhez**</span><span class="sxs-lookup"><span data-stu-id="7964a-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="7964a-104">Olvassa el [ezt a cikket](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span><span class="sxs-lookup"><span data-stu-id="7964a-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="7964a-105">[Adjon hozzá Intune licencet a felhasználóknak](https://docs.microsoft.com/intune/licenses-assign).</span><span class="sxs-lookup"><span data-stu-id="7964a-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="7964a-106">A Társtulajdonkezelés konfigurálásakor használja a [szegélyböngészőt](https://www.microsoft.com/windows/microsoft-edge) .</span><span class="sxs-lookup"><span data-stu-id="7964a-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="7964a-107">**Hogyan kell telepíteni a config Manager kliens Intune-vezérelt eszközök**</span><span class="sxs-lookup"><span data-stu-id="7964a-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="7964a-108">További információ: [Intune MDM-kezelt Windows-eszközök](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span><span class="sxs-lookup"><span data-stu-id="7964a-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="7964a-109">**Mi van, ha én csak azt szeretném változtatni MDM hatóság?**</span><span class="sxs-lookup"><span data-stu-id="7964a-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="7964a-110">Az MDM hatóság támogatási eset megnyitása nélkül is megváltoztatható.</span><span class="sxs-lookup"><span data-stu-id="7964a-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="7964a-111">Kérjük, olvassa el az alábbi dokumentációt, hogy segítse az MDM hatóság megváltoztatását:</span><span class="sxs-lookup"><span data-stu-id="7964a-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="7964a-112">MDM hatóság módosítása a Konfigurációkezelőtől az Intune önálló</span><span class="sxs-lookup"><span data-stu-id="7964a-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="7964a-113">Változás MDM hatóság Intune önálló config Manager</span><span class="sxs-lookup"><span data-stu-id="7964a-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)