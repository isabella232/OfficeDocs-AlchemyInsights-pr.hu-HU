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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003391"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Az örökölt párbeszédpanelek beágyazásának engedélyezése jelentések megnyitásához

**Jelenség**

A felhasználók nem tudnak jelentéseket megnyitni. „Valami hiba történt. További részletekért tekintse meg a technikai adatokat.”

**Ok**

A jelentések betöltése sikertelen az UCI-ben „Az űrlapleíró null érték vagy nincs megadva“ hibaüzenettel. Az UCI-beli jelentésekhez továbbra is szükségesek az örökölt párbeszédpanelek, így az ügyfélrendszernek engedélyeznie kell az *allowlegacydialogsembedding* beállítást.

**Megoldás**

1. Válassza a **Beállítások >Felügyelet > Rendszerbeállítások > Általános lap** lehetőséget.

2. Állítsa az "Egyes örökölt párbeszédpanelek beágyazásának engedélyezése az Egyesített felület böngészőprogramban" beállítást **Igen** értékre.
