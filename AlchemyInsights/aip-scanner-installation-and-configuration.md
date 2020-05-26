---
title: 'AIP szkenner: telepítés és konfigurálás'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358098"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="d0896-102">AIP szkenner: telepítés és konfigurálás</span><span class="sxs-lookup"><span data-stu-id="d0896-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="d0896-103">**Az AIP-képolvasó telepítéséhez kövesse az ajánlott irányelveket:**</span><span class="sxs-lookup"><span data-stu-id="d0896-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="d0896-104">Ha frissítést frissít, és nem végez tiszta telepítést, győződjön meg arról, hogy betartotta [az Azure Information Protection képolvasó és az](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) egyesített címkézési ügyfél frissítésére vonatkozó irányelveket, olvassa el az Azure Information Protection [képolvasó frissítése](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)című témakört.</span><span class="sxs-lookup"><span data-stu-id="d0896-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="d0896-105">Ellenőrizze, hogy megfelel-e a [tűzfalakra és a hálózati infrastruktúra beállításaira vonatkozó összes követelménynek.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="d0896-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="d0896-106">Győződjön meg arról, hogy a házirendek automatikus [címkézésre vannak beállítva,](https://docs.microsoft.com/azure/information-protection/configure-policy) vagy alapértelmezett címkével rendelkeznek a házirendben.</span><span class="sxs-lookup"><span data-stu-id="d0896-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="d0896-107">Győződjön meg arról, hogy a megfelelő fájltípus az [Azure Information Protection ügyfél által támogatott fájltípusokban](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)leírtak szerint van konfigurálva a címkén/védelemben.</span><span class="sxs-lookup"><span data-stu-id="d0896-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="d0896-108">Ezenkívül, ha módosítani szeretné az alapértelmezett viselkedést, kövesse az alábbi irányelveket: [A fájlok alapértelmezett védelmi szintjének módosítása](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="d0896-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="d0896-109">Ellenőrizze, hogy a lapolvasó szolgáltatás futtatására beállított felhasználói fiók rendelkezik-e az összes konfigurált tárház elérésére vonatkozó engedéllyel.</span><span class="sxs-lookup"><span data-stu-id="d0896-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="d0896-110">Ha továbbra is problémákat tapasztal, exportálja a lapolvasó naplókat, és adja hozzá őket a támogatási jegyhez.</span><span class="sxs-lookup"><span data-stu-id="d0896-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="d0896-111">**Az Azure Information Protection Scanner naplóinak exportálása**</span><span class="sxs-lookup"><span data-stu-id="d0896-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="d0896-112">Keresse meg a %localappdata%\Microsoft\MSIP mappát a képolvasó szolgáltatást futtató felhasználói környezetben.</span><span class="sxs-lookup"><span data-stu-id="d0896-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="d0896-113">Zip minden tartalmát az MSIP mappába.</span><span class="sxs-lookup"><span data-stu-id="d0896-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="d0896-114">Mentse a naplókat a választott helyre, és csatolja őket a szolgáltatási kérelemhez.</span><span class="sxs-lookup"><span data-stu-id="d0896-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="d0896-115">Használhatja [az Export-AIPLogs -OnBehalfOf parancsot](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)is.</span><span class="sxs-lookup"><span data-stu-id="d0896-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="d0896-116">**További információ:**</span><span class="sxs-lookup"><span data-stu-id="d0896-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="d0896-117">Az Azure Information Protection képolvasó telepítése a fájlok automatikus besorolásához és védelméhez</span><span class="sxs-lookup"><span data-stu-id="d0896-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="d0896-118">A Token paraméter megadása és használata a Set-AIPAuthentication paraméterhez</span><span class="sxs-lookup"><span data-stu-id="d0896-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="d0896-119">Felderítési ciklus futtatása és jelentések megtekintése a képolvasóhoz</span><span class="sxs-lookup"><span data-stu-id="d0896-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="d0896-120">Tekintse át az Azure Information Protection dokumentációját</span><span class="sxs-lookup"><span data-stu-id="d0896-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d0896-121">Az Azure-információvédelem követelményei</span><span class="sxs-lookup"><span data-stu-id="d0896-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="d0896-122">Az Azure Information Protection ügyfél letöltése</span><span class="sxs-lookup"><span data-stu-id="d0896-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
