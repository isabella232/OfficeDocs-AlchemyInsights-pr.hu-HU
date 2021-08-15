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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013750"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Az Apple automatikus eszközregisztrációs szinkronizálási hibái

"Azt észleltük, hogy egy vagy több ADE/DEP-tokenje van, amelyek hibaállapotban vannak. Amíg meg nem oldja a hibaállapotot az egyes érintett tokenek esetén, az ADE-funkció nem a várt módon fog működni."

Ez a hiba számos módon jelentkezhet, például:

1. Előfordulhat, hogy az eszközök nem szinkronizálódnak az ABM/ASM eszközről az Intune-ba
2. A regisztrációs profil hozzárendelései sikertelenek lehetnek
3. Előfordulhat, hogy az eszközök nem fejeződnek be sikeresen az ADE-regisztráción

Ellenőrizze, hogy nincs-e az Intune konzolon jelentett szinkronizálási hiba az Eszközök > **Az Apple-regisztráció**> és a Regisztrációs program > eszköz alatt.

A szinkronizálási hiba egyik leggyakoribb oka az aktuális jogkivonat lejárata. Az érintett jogkivonat megújítása sok esetben megoldja a problémát.

Ha egy vagy több tokenje lejárt, az alábbi dokumentációban segítséget találhat a tokenek szükség szerint való megújításának segítése érdekében:

[Automatikus eszközregisztrációs jogkivonat megújítása](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Ezenkívül az alábbi dokumentációban láthatja a tokenszinkronizálási hibákat okozó egyéb hibák esetleges szervizelését:

[ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
