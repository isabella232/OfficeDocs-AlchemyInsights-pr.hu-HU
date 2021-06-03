---
title: Eszközcímkék és -csoportok létrehozása és kezelése
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
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731666"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="367be-102">Eszközcímkék és -csoportok létrehozása és kezelése</span><span class="sxs-lookup"><span data-stu-id="367be-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="367be-103">Az eszközökön címkéket hozzáadva logikai csoportfedéseket hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="367be-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="367be-104">Az eszközcímkék támogatják a hálózat megfelelő megfeleltetését, lehetővé téve különböző címkék csatolását a környezet rögzítése és a dinamikus listakészítés engedélyezése egy incidens részeként.</span><span class="sxs-lookup"><span data-stu-id="367be-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="367be-105">A címkék használhatók szűrőként az Eszközök listanézetben, illetve eszközök csoportosításához.</span><span class="sxs-lookup"><span data-stu-id="367be-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="367be-106">Az eszközcsoportozásról további információt az Eszközcímkék létrehozása és [kezelése lapon található.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="367be-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="367be-107">Az eszközökön a következő eszközökkel adhat hozzá címkéket:</span><span class="sxs-lookup"><span data-stu-id="367be-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="367be-108">A portál használata</span><span class="sxs-lookup"><span data-stu-id="367be-108">Using the portal</span></span>

- <span data-ttu-id="367be-109">Beállításkulcsérték beállítása</span><span class="sxs-lookup"><span data-stu-id="367be-109">Setting a registry key value</span></span>
 
<span data-ttu-id="367be-110">**Megjegyzés:** Késés lehet az eszköz címkéinek az eszközre való hozzáadása és az eszközlistában és az eszközlapon való elérhetősége között.</span><span class="sxs-lookup"><span data-stu-id="367be-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="367be-111">Az eszközcímkék API-val való hozzáadásáról az Eszközcímkék API hozzáadása vagy [eltávolítása .](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="367be-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="367be-112">Eszközcímkék hozzáadása és kezelése a portálon</span><span class="sxs-lookup"><span data-stu-id="367be-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="367be-113">Válassza ki azt az eszközt, amelyről a címkéket kezelni szeretné.</span><span class="sxs-lookup"><span data-stu-id="367be-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="367be-114">Az eszközt az alábbi nézetek bármelyikében választhatja ki vagy keresheti meg:</span><span class="sxs-lookup"><span data-stu-id="367be-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="367be-115">**Biztonsági műveletek irányítópultja** Válassza ki az eszköz nevét a Legnépszerűbb eszközök aktív riasztásokkal szakaszban.</span><span class="sxs-lookup"><span data-stu-id="367be-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="367be-116">**Riasztási várólista** – Válassza ki az eszköz nevét az eszköz ikonja mellett a riasztási várólistán.</span><span class="sxs-lookup"><span data-stu-id="367be-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="367be-117">**Eszközök lista** – Válassza ki az eszköz nevét az eszközlistából.</span><span class="sxs-lookup"><span data-stu-id="367be-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="367be-118">**Keresőmező –** Válassza az Eszköz elemet a legördülő menüből, és írja be az eszköz nevét.</span><span class="sxs-lookup"><span data-stu-id="367be-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="367be-119">A riasztási lapot a fájl- és IP-nézetekben is meg tudja jelenni.</span><span class="sxs-lookup"><span data-stu-id="367be-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="367be-120">A **Válaszműveletek sorában** válassza a Címkék kezelése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="367be-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="367be-121">Írjon be címkéket a kereséshez vagy a létrehozáshoz.</span><span class="sxs-lookup"><span data-stu-id="367be-121">Type to find or create tags.</span></span>

<span data-ttu-id="367be-122">A címkék bekerülnek az eszköznézetbe, és megjelennek az Eszközök listanézetben.</span><span class="sxs-lookup"><span data-stu-id="367be-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="367be-123">Ezután a Címkék szűrővel láthatja a megfelelő eszközlistát.</span><span class="sxs-lookup"><span data-stu-id="367be-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="367be-124">További információ: [Eszközcímkék létrehozása és kezelése.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="367be-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>