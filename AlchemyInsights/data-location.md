---
title: Adathely
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207263"
---
# <a name="data-location"></a>Adathely

Tudod kilátás a elhelyezés-ból-a Hivatal 365 bérlő-ban admin központ vagy mellett összekötő pálca-hoz cserél online keresztül PowerShell.


**Admin központ:**
1. Jelentkezz be az [Admin Centerbe](https://admin.microsoft.com/Adminportal/Home).
2. Válassza a **Beállítások** > **szervezeti profilja**beállítást.
3. Az **adathely**területen válassza a **nézet részletei nézetet**.


**Powershell:**
1. Csatlakozzon az Exchange Online rendszerhez a Windows PowerShell eszközzel.
2. A bérlő tulajdonságainak listájának megjelenítéséhez futtassa a [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) parancsmagot. 
3. Tekintse meg a OrganizationId tulajdonságot.

Az EXO és az SPO adathelyének meghatározásához meghatározhatja, hogy az adatok [Hol találhatók az adott](https://products.office.com/where-is-your-data-located)helyen.