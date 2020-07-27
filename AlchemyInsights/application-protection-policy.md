---
title: Alkalmazásvédelmi házirend
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423598"
---
# <a name="application-protection-policy"></a>Alkalmazásvédelmi házirend

Ha most nem találja az alkalmazásvédelmi szabályzatot (APP), olvassa el az [alkalmazásvédelmi szabályzatok áttekintését.](https://docs.microsoft.com/intune/apps/app-protection-policy)

Az APP használatának megkezdéséhez olvassa el [Az alkalmazásvédelmi szabályzatok létrehozása és hozzárendelése című témakört.](https://docs.microsoft.com/intune/app-protection-policies)

Alkalmazásvédelmi házirend követelményei:

- A felhasználó Intune- vagy EMS-licenccel rendelkezik.
- A felhasználó az alkalmazásvédelmi házirendek által megcélzott csoporthoz tartozik.
- Csak egy vállalati felhasználó van bejelentkezve a védett alkalmazásokba az eszközön.
- Az alkalmazás megvalósította az [Intune SDK-t.](https://docs.microsoft.com/intune/app-sdk-get-started) Az SDK-t támogató alkalmazások listáját a [Microsoft Intune által védett alkalmazások](https://docs.microsoft.com/intune/apps-supported-intune-apps)című témakörben tetszésszerint.

A szabályzatok azt követően érvényesek, hogy egy felhasználó, aki megfelel a fenti követelményeknek, bejelentkezik egy Intune SDK-kompatibilis alkalmazásba. A házirend alkalmazásának legegyszerűbb módja, ha megkell követelni, hogy a felhasználó pin-kódot állítson be a házirendben. 

További információ:

[APP/MAM hibaelhárítás – gyakori kérdések](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Az alkalmazásvédelmi szabályzat beállításának ellenőrzése](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Az alkalmazásvédelmi szabályzat kézbesítési ütemezésének ismertetése](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Az alkalmazásvédelmi szabályzatok figyelése](https://docs.microsoft.com/intune/app-protection-policies-monitor)