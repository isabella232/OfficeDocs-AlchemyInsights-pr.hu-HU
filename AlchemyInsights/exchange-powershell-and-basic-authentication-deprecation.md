---
title: Az Exchange PowerShell és az egyszerű hitelesítés elévülése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015691"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Az Exchange PowerShell és az egyszerű hitelesítés elévülése

Ha további információra van szüksége arról, hogy miként csatlakozhat az Exchange Online PowerShellhez egyszerű hitelesítés használata nélkül, [látogasson el ide](https://aka.ms/psbasicauth).

Felhívjuk a figyelmét arra, hogy az egyszerű hitelesítésnek továbbra is engedélyezve kell lennie az ügyfélgépen.
Az új PowerShell V2 modul modern hitelesítés használatával létesít kapcsolatot, hogy lehetővé tegye az összes REST-alapú V2-es parancsmag használatát. A V2-es parancsmagok használata mellett ez azt is lehetővé teszi, hogy elérjék a régebbi Távoli PowerShell-parancsmagokat (RPS), amelyekhez Távoli PowerShell-munkamenetet kell létesíteni. Ahhoz, hogy RPS-munkamenetet létesítsenek Windows rendszerű gépen, a WinRM egyszerű hitelesítésnek engedélyezve kell lennie az ügyfélgépen annak ellenére, hogy a modul modern hitelesítési mechanizmust használ a szolgáltatás felé történő hitelesítéshez. A rendszer a WinRM egyszerű hitelesítés csatornáját használja a modern hitelesítés jogkivonatainak továbbítására. Ha a WinRM egyszerű hitelesítés le van tiltva az ügyfélgépen, az új V2-es parancsmagok továbbra is működni fognak (a régebbi RPS-parancsmagok azonban nem).
