---
title: Az örökölt párbeszédpanelek beágyazásának engedélyezése jelentések megnyitásához
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814266"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Az örökölt párbeszédpanelek beágyazásának engedélyezése jelentések megnyitásához

**Jelenség**

A felhasználók nem tudnak jelentéseket megnyitni. „Valami hiba történt. További részletekért tekintse meg a technikai adatokat.”

**Ok**

A jelentések betöltése sikertelen az UCI-ben „Az űrlapleíró null érték vagy nincs megadva“ hibaüzenettel. Az UCI-beli jelentésekhez továbbra is szükségesek az örökölt párbeszédpanelek, így az ügyfélrendszernek engedélyeznie kell az *allowlegacydialogsembedding* beállítást.

**Megoldás**

1. Válassza a **Beállítások >Felügyelet > Rendszerbeállítások > Általános lap** lehetőséget.

2. Állítsa az "Egyes örökölt párbeszédpanelek beágyazásának engedélyezése az Egyesített felület böngészőprogramban" beállítást **Igen** értékre.
