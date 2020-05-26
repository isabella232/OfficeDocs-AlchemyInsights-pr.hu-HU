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
# <a name="aip-scanner-installation-and-configuration"></a>AIP szkenner: telepítés és konfigurálás

**Az AIP-képolvasó telepítéséhez kövesse az ajánlott irányelveket:**

1. Ha frissítést frissít, és nem végez tiszta telepítést, győződjön meg arról, hogy betartotta [az Azure Information Protection képolvasó és az](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) egyesített címkézési ügyfél frissítésére vonatkozó irányelveket, olvassa el az Azure Information Protection [képolvasó frissítése](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)című témakört.
2. Ellenőrizze, hogy megfelel-e a [tűzfalakra és a hálózati infrastruktúra beállításaira vonatkozó összes követelménynek.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Győződjön meg arról, hogy a házirendek automatikus [címkézésre vannak beállítva,](https://docs.microsoft.com/azure/information-protection/configure-policy) vagy alapértelmezett címkével rendelkeznek a házirendben.
4. Győződjön meg arról, hogy a megfelelő fájltípus az [Azure Information Protection ügyfél által támogatott fájltípusokban](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)leírtak szerint van konfigurálva a címkén/védelemben. Ezenkívül, ha módosítani szeretné az alapértelmezett viselkedést, kövesse az alábbi irányelveket: [A fájlok alapértelmezett védelmi szintjének módosítása](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Ellenőrizze, hogy a lapolvasó szolgáltatás futtatására beállított felhasználói fiók rendelkezik-e az összes konfigurált tárház elérésére vonatkozó engedéllyel.
6. Ha továbbra is problémákat tapasztal, exportálja a lapolvasó naplókat, és adja hozzá őket a támogatási jegyhez.

**Az Azure Information Protection Scanner naplóinak exportálása**

1. Keresse meg a %localappdata%\Microsoft\MSIP mappát a képolvasó szolgáltatást futtató felhasználói környezetben.
2. Zip minden tartalmát az MSIP mappába.
3. Mentse a naplókat a választott helyre, és csatolja őket a szolgáltatási kérelemhez.
4. Használhatja [az Export-AIPLogs -OnBehalfOf parancsot](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)is.

**További információ:**
- [Az Azure Information Protection képolvasó telepítése a fájlok automatikus besorolásához és védelméhez](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [A Token paraméter megadása és használata a Set-AIPAuthentication paraméterhez](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Felderítési ciklus futtatása és jelentések megtekintése a képolvasóhoz](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Tekintse át az Azure Information Protection dokumentációját](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Az Azure-információvédelem követelményei](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Az Azure Information Protection ügyfél letöltése](https://www.microsoft.com/download/details.aspx?id=53018)
