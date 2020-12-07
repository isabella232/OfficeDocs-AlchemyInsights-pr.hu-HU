---
title: Mi a teendő, ha az Azure-funkciók nem működnek megfelelően a Microsoft Edge-ben
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583460"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Mi a teendő, ha az Azure-funkciók nem működnek megfelelően a Microsoft Edge-ben

A Microsoft Edge [ismert problémákkal](https://go.microsoft.com/fwlink/?linkid=2140608) bír, amelyek a biztonsági zónákhoz kapcsolódnak, és befolyásolhatják, hogy az Azure-felhasználók hogyan jelentkezzenek be a Windows felügyeleti központba. Ha problémát tapasztal az Azure-funkciók Microsoft Edge-ben való használatakor, próbálkozzon az alábbi lépésekkel:

1. A **Start** menüben keresse meg az **Internetbeállítások lehetőséget** , és jelölje ki.
2. Az **Internet tulajdonságai** párbeszédpanelen lépjen a **Biztonság** lapra.
3. Jelölje ki a **megbízható helyek** zónát, és válassza a **webhelyek** gombot.
4. A **megbízható helyek** párbeszédpanelen adja meg az átjáró URL-címét, és [https://login.microsoftonline.com](https://login.microsoftonline.com) válassza a [https://login.live.com](https://login.live.com) **Bezárás** gombot.
5. Az **Internet tulajdonságai** párbeszédpanelen lépjen az **Adatvédelem** lapra.
6. Az **előugró ablakok blokkolása** csoportban válassza a **Beállítások** lehetőséget. A megnyíló párbeszédpanelen adja meg az átjáró URL-címét, és [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) válassza a **Bezárás** gombot.
