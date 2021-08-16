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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067842"
---
# <a name="gpo-deployment"></a>GPO-telepítés

Gépház Azure Active Directory tartományi szolgáltatásokban (Azure AD DS) lévő felhasználói és számítógépes objektumokat gyakran kezelik csoportházirend-objektumok (GPOS-k) használatával. Az Azure AD DS beépített GPOS-eket tartalmaz az AADDC-felhasználók és az AADDC számítógépek tárolóihoz. Ezeket a beépített CSOPORTHÁZIREND-objektumokat testre szabhatja úgy, hogy a környezetéhez szükséges csoportházirendeket konfigurálja. Az Azure AD DC rendszergazdák csoportjának tagjai csoportházirend-felügyeleti jogosultságokkal az Azure AD DS tartományban, valamint egyéni csoportházirend-objektumokat és szervezeti egységeket is létrehozhatnak. A csoportházirendek működése és működése a Csoportházirendek áttekintése [témakörben található.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Hibrid környezetben a helyszíni AD DS-környezetben konfigurált csoportházirendek nem szinkronizálódnak az Azure AD DS szolgáltatásba. Az Azure AD DS-felhasználók és számítógépek konfigurációs beállításainak meghatározásához szerkessze az egyik alapértelmezett csoportházirend-objektumát, vagy hozzon létre egyéni csoportházirend-objektumokat.

Ebből a [csoportházirend-kezelésről](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) ebben a cikkben olvashat arról, hogy miként telepítheti a csoportházirend-kezelő eszközöket, hogyan szerkesztheti a beépített gposokat, és hogyan hozhat létre egyéni CSOPORTHÁZIREND-objektumokat.
