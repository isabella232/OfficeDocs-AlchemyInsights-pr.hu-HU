---
title: Listaelemek megjegyzései
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995489"
---
# <a name="comments-on-list-items"></a>Listaelemek megjegyzései

A felhasználók megtekinthetik egy listaelem összes megjegyzését, és szűrhet az elemekhez kapcsolódó megjegyzéseket vagy tevékenységeket bemutató nézetek között.

A megjegyzés hozzáadásához és törléséhez a felhasználóknak fel kelljegyeni az alábbiakat:

- A megjegyzések a megjegyzésekben rejlő engedélybeállításokat SharePoint.
- A modern felhasználói felületeken ( például feladatlistákon) még nem látható klasszikus listákban nem található meg ez a megjegyzési funkció.
- Ebben a kiadásban nem lehet megjegyzéseket Teams listákhoz.
- A keresés nem indexeli a megjegyzéseket.

A rendszergazdák szervezetszinten letilthatják ezt a szolgáltatást a **Set-SPOTenant** PowerShell-parancsmag **CommentsOnListItemsDisabled** paraméterének módosításával.

A megjegyzések webhely vagy lista szintjén jelenleg nem tiltható le. Reményeink szerint a vezérlőket egy későbbi frissítésben, valószínűleg a 2021 első negyedévében is elérhetővé tejük.
