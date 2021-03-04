---
title: Az Apple automatikus eszközregisztrációs szinkronizálási hibái
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448924"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Az Apple automatikus eszközregisztrációs szinkronizálási hibái

"Azt észleltük, hogy egy vagy több ADE/DEP-tokenje van, amelyek hibaállapotban vannak. Amíg meg nem oldódik az egyes érintett jogkivonatok hibaállapota, az ADE-funkció nem a várt módon fog működni."

Ez a hiba többféleképpen jelenhet meg:

1. Előfordulhat, hogy az eszközök nem szinkronizálódnak az ABM/ASM eszközről az Intune-ba
2. Előfordulhat, hogy sikertelenek a regisztrációs profil hozzárendelései
3. Előfordulhat, hogy az eszközök nem fejeződnek be sikeresen az ADE-regisztrációval

Ellenőrizze, hogy nincs-e az Intune konzolon jelentett szinkronizálási hiba az Eszközök > eszköz regisztrálása > Az Apple regisztrációs > **regisztrációs program jogkivonatai között.**

A szinkronizálási hiba egyik leggyakoribb oka az aktuális jogkivonat lejárata. Az érintett jogkivonat megújítása sok esetben megoldja a problémát.

Ha egy vagy több tokenje lejárt, az alábbi dokumentációban segítséget talál a tokenek szükség szerint való megújításának segítése érdekében:

[Automatikus eszközregisztrációs jogkivonat megújítása](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Ezenkívül az alábbi dokumentációban láthatja a jogkivonat-szinkronizálási hibákat okozó egyéb hibák esetleges szervizelését:

[ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
