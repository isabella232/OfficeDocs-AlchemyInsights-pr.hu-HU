---
title: Bérlői házirend kijavítása (művelet felülbírálása)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694062"
---
# <a name="fix-tenant-policy-action-override"></a>Bérlői házirend kijavítása (művelet felülbírálása)

Ezt az üzenetet egy levélszemét-szűrési házirend érintette a bérlői webhelyen. A házirend áttekintéshez tegye a következőket:

1. Válassza az [Office 365 Biztonsági & megfelelőségi központot,](https://go.microsoft.com/fwlink/p/?linkid=2077143)majd a   >  Veszélyforrás-kezelési **házirend** levélszemét elleni  >  [védelem szolgáltatását.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Ellenőrizze, hogy  a házirendforrás a következőt **jelzi-e: Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Ha igen, az Egyéni **lapon** ellenőrizze az üzenetre vonatkozó házirend beállításait. Lehetséges, hogy az  Exchange Online Védelmi szolgáltatás minden ügyfele számára érvényes szokásos beállítások hatással vannak az üzenetre.

A levélszemétszűrő házirendek konfigurálásával kapcsolatos további információkért [lásd: A levélszemétszűrő házirendek konfigurálása.](https://go.microsoft.com/fwlink/?linkid=2101431)
