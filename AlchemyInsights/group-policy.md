---
title: Csoportházirend
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256778"
---
# <a name="group-policy"></a>Csoportházirend

Az Azure Active Directory tartományi szolgáltatásokban (Azure AD DS) lévő felhasználói és számítógépes objektumok beállításait gyakran csoportházirend-objektumok (GPOs) használatával kezelik. Az Azure AD DS beépített CSOPORTHÁZIREND-objektumokat tartalmaz az AADDC-felhasználók és az AADDC számítógépek tárolóihoz. Ezeket a beépített csoportházirend-objektumokat testre szabhatja úgy, hogy a környezetéhez szükség szerint konfigurálja a csoportházirendeket. Az Azure AD DC rendszergazdák csoportjának tagjai csoportházirend-felügyeleti jogosultságokkal az Azure AD DS tartományban, valamint egyéni csoportházirend-objektumokat és szervezeti egységeket is létrehozhatnak. A csoportházirendek szerkezetét és működését a Csoportházirend áttekintése [témakörben olvashatja.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Hibrid környezetben a helyszíni AD DS-környezetben konfigurált csoportházirendek nem szinkronizálódnak az Azure AD DS szolgáltatásba. Ha konfigurációs beállításokat ad meg az Azure AD DS felhasználóinak vagy számítógépein, szerkessze az egyik alapértelmezett csoportházirend-objektumát, vagy hozzon létre egy egyéni csoportházirend-objektumát.

Ez a cikk a [csoportházirendek](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) kezelését mutatja be, hogy miként telepítheti a csoportházirend-kezelő eszközöket, hogyan módosíthatja a beépített csoportházirend-objektumokat, és hogyan hozhat létre egyéni csoportházirend-objektumokat.



