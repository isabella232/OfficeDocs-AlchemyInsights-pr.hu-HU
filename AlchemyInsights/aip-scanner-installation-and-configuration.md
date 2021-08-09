---
title: 'AIP-képolvasó: telepítés és konfiguráció'
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
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934259"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-képolvasó: telepítés és konfiguráció

**Az AIP-képolvasó telepítéséhez kövesse a következő ajánlott irányelveket:**

1. Ha frissítés alatt áll, és nem végez tiszta telepítést, kérjük, hogy az [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) scanner frissítésére és az egységes címkézést végző ügyfélprogramra vonatkozó irányelveket az Azure Information [Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)scanner frissítésével kapcsolatos útmutatásnak megfelelően végezze el.
2. Ellenőrizze, hogy megfelel-e a [tűzfalak és a hálózati infrastruktúra minden beállítási követelményének.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Győződjön meg arról, hogy [a házirendek](https://docs.microsoft.com/azure/information-protection/configure-policy) automatikus feliratozásra vannak beállítva, vagy hogy a házirendben van alapértelmezett címke.
4. Győződjön meg arról, hogy a megfelelő fájltípus a felirat/védelem beállítását ismerteti az Azure Information Protection-ügyfél által támogatott fájltípusok [leírásának megfelelően.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Ezenkívül ha meg szeretné változtatni az alapértelmezett viselkedést, kövesse a következő irányelveket: A fájlok alapértelmezett védelmi szintjének [módosítása.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Győződjön meg arról, hogy a képolvasó szolgáltatás futtatására konfigurált felhasználói fiók rendelkezik az összes beállított tár eléréséhez szükséges engedélyekkel.
6. Ha továbbra is problémákat tapasztal, exportálja a szkennernaplókat, és vegye fel őket a támogatási jegybe.

**Azure Information Protection Scanner-naplók exportálása**

1. Keresse meg a %localappdata%\Microsoft\MSIP parancsot a képolvasó szolgáltatást futtató felhasználói környezetben.
2. Tömörítsen minden tartalmat az MSIP mappában.
3. Mentse a naplókat a választott helyre, és csatolja őket a szolgáltatáskéréshez.
4. Használhatja az [Export-AIPLogs -OnBehalfOf használhatja is.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**További információ:**
- [Az Azure Information Protection szkenner központi telepítése a fájlok automatikus osztályozásához és védelméhez](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [A Token paraméter megadása és használata a Set-AIPAuthentication paraméterhez](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Feltárási ciklus futtatása és a képolvasó jelentésének megtekintése](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Az Azure Information Protection dokumentációjának áttekintése](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Az Azure Information Protection követelményei](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Az Azure Information Protection-ügyfél letöltése](https://www.microsoft.com/download/details.aspx?id=53018)
