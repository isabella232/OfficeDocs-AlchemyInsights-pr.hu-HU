---
title: Az Apple automatikus eszköz-beiktatási szinkronizálási hibái
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714833"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Az Apple automatikus eszköz-beiktatási szinkronizálási hibái

"Észlelték, hogy egy vagy több ADE/DEP-token van, ami egy hibás állapotú. Mindaddig, amíg a hiba állapotát meg nem oldotta az egyes érintett jogkivonatok esetében, az ADE-funkció nem fog működni.

Ez a hiba többféle módon nyilvánulhat meg, többek között az alábbiakat:

1. Lehet, hogy az eszközök nem szinkronizálhatók az ABM/ASM rendszerből a Intune-ra
2. Lehet, hogy sikertelenek a tanúsítványigénylési profil hozzárendelései
3. Az eszközök nem feltétlenül fejezik be az ADE-regisztrációt

Ellenőrizze, hogy milyen szinkronizálási hibáról van-e lehetőség a Intune-konzolban az **eszközök > > az Apple tanúsítványigénylési > a beiratkozási program-tokenek** csoportban, és tekintse át az alábbi dokumentumokat a potenciális kármentesítés megtekintéséhez:

[ABM/ASM szinkronizálási hibák az iOS/iPadOS és a macOS automatikus eszköz-igénylési tokenek esetén](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
