---
title: Az Exchange PowerShell és az egyszerű hitelesítés elévülése
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813474"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Az Exchange PowerShell és az egyszerű hitelesítés elévülése

Ha további információra van szüksége arról, hogy miként csatlakozhat az Exchange Online PowerShellhez egyszerű hitelesítés használata nélkül, [látogasson el ide](https://aka.ms/exops-docs). A PowerShell V2 modul nem használ egyszerű hitelesítést.

Felhívjuk a figyelmét arra, hogy az egyszerű hitelesítésnek továbbra is engedélyezve kell lennie az ügyfélgépen.
Az új PowerShell V2 modul modern hitelesítés használatával létesít kapcsolatot, hogy lehetővé tegye az összes REST-alapú V2-es parancsmag használatát. A V2-es parancsmagok használata mellett ez azt is lehetővé teszi, hogy elérjék a régebbi Távoli PowerShell-parancsmagokat (RPS), amelyekhez Távoli PowerShell-munkamenetet kell létesíteni. Ahhoz, hogy RPS-munkamenetet létesítsenek Windows rendszerű gépen, a WinRM egyszerű hitelesítésnek engedélyezve kell lennie az ügyfélgépen annak ellenére, hogy a modul modern hitelesítési mechanizmust használ a szolgáltatás felé történő hitelesítéshez. A rendszer a WinRM egyszerű hitelesítés csatornáját használja a modern hitelesítés jogkivonatainak továbbítására. Ha a WinRM egyszerű hitelesítés le van tiltva az ügyfélgépen, az új V2-es parancsmagok továbbra is működni fognak (a régebbi RPS-parancsmagok azonban nem).
