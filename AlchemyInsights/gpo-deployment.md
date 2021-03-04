---
title: GPO-telepítés
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427569"
---
# <a name="gpo-deployment"></a>GPO-telepítés

Az Azure Active Directory tartományi szolgáltatásokban (Azure AD DS) található felhasználói és számítógépes objektumok beállításait gyakran csoportházirend-objektumok (GPOs) használatával kezelik. Az Azure AD DS beépített CSOPORTHÁZIREND-objektumokat tartalmaz az AADDC-felhasználók és az AADDC számítógépek tárolóihoz. Ezeket a beépített csoportházirend-objektumokat testre szabhatja úgy, hogy a környezetéhez szükség szerint konfigurálja a csoportházirendeket. Az Azure AD DC rendszergazdák csoportjának tagjai csoportházirend-felügyeleti jogosultságokkal az Azure AD DS tartományban, valamint egyéni csoportházirend-objektumokat és szervezeti egységeket is létrehozhatnak. A csoportházirendek szerkezetét és működését a Csoportházirendek áttekintése [témakörben olvashatja.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Hibrid környezetben a helyszíni AD DS-környezetben konfigurált csoportházirendek nem szinkronizálódnak az Azure AD DS szolgáltatásba. Ha konfigurációs beállításokat ad meg az Azure AD DS felhasználóinak vagy számítógépein, szerkessze az egyik alapértelmezett csoportházirend-objektumát, vagy hozzon létre egy egyéni csoportházirend-objektumát.

Ez a [csoportházirend-kezelésről](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) készült cikk bemutatja, hogy miként telepítheti a csoportházirend-kezelő eszközöket, hogyan módosíthatja a beépített csoportházirend-objektumokat, és hogyan hozhat létre egyéni csoportházirend-objektumokat.
