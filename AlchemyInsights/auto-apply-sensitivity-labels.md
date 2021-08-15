---
title: Bizalmasság-címkék automatikus alkalmazása
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1737"
- "9000181"
ms.openlocfilehash: 7a32ad52f115b9ada40f7cd47c90ceb3dcd3f9cd99a8f9eae3514b2e45e73bb8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969294"
---
# <a name="auto-apply-sensitivity-labels"></a>Bizalmasság-címkék automatikus alkalmazása

Tartalmi címkéket manuálisan is alkalmazhatók a felhasználók a tartalomra, vagy beállíthatja, hogy automatikusan alkalmazza őket a tartalomra.

Tartalmi címkék automatikus alkalmazása esetén nem kell képzéseket alkalmazni a felhasználóknak a tartalom osztályozására és a házirend-konfigurációkról való értesítésre.

A címkék automatikus alkalmazásához az alábbiakra van szükség:

- Azure Information Protection P2-előfizetés
- [Az Azure Information Protection egységes címkézési ügyfélprogram letöltése és telepítése](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

Dolgozunk azon a natív támogatáson, amely a jövőben nem igényli az Azure Information Protection egységes címkéző ügyfélprogramját.

Jelenleg csak a Windows támogatja az egyesített címkézési ügyfélalkalmazást.  A funkció Még nem támogatott Macen, iOS-en és Androidon.

A tartalmi címkékről és azok tartalomra való automatikus alkalmazásával kapcsolatos további információkért lásd:

- [A bizalmasság-címkék áttekintése](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [Tartalom automatikus alkalmazása tartalomra](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically)