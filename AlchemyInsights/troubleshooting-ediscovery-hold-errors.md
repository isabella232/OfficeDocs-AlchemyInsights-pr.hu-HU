---
title: Hibakeresési hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676151"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Hibakeresési hibák elhárítása

Problémákat tapasztal adiscovery-visszavételekkel kapcsolatban? Íme néhány ajánlott eljárás, amit érdemes megfontolni:

- Ellenőrizze a terjesztés állapotát.  Ha az állapot **Be (függőben)** vagy Ki **(függőben)** állapotú, várja meg, amíg befejeződik a terjesztés.
- A frissítéseket egyetlen tömeges kérésben egyesítheti, nem kell minden tranzakcióhoz ismétlődően frissítenie a házirendet.
- Futtassa Set-CaseHoldPolicy <policyname> -RetryDistribution parancsot a Biztonsági és megfelelőségi központ Powershellben. További információt a Biztonsági [Csatlakozás PowerShell & olvashat.](/powershell/exchange/connect-to-scc-powershell)

A beállítások ellenőrzéséhez szükséges lépéseket, valamint az elektronikus adatok visszavételével kapcsolatos hibák megoldását és megoldását bemutató további gyakorlati tanácsokért lásd: A elektronikus adatok visszavételével kapcsolatos [hibák elhárítása.](/microsoft-365/compliance/hold-distribution-errors)
Az egyéb gyakori adatfeladatokat és hibák elhárítását a Gyakori adatfelkeresési problémák felderítése, hibaelhárítása és megoldása témakörben [kaphatja meg.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
