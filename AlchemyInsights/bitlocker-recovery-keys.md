---
title: Bitlocker helyreállítási kulcsok
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060066"
---
# <a name="accessing-bitlocker-recovery-keys"></a>A Bitlocker helyreállítási kulcsok elérése

A Bitlocker-beállítások Intune Endpoint Protection-házirend konfigurálásakor megadhatja, hogy a Bitlocker helyreállítási információkat tárolja-e a Azure Active Directory.

Ha ez a beállítás be van állítva, akkor a tárolt helyreállítási adatoknak az Intune-rendszergazdáknak az Intune Devices blade eszközben tárolt eszközrekord-adatok részeként két módon kell láthatónak lenniük:

Eszközök – Azure AD-eszközök –> "Eszköz" VAGY Eszközök -> Minden eszköz -> "Eszköz" -> helyreállítási kulcsok

Ha maga az eszköz rendszergazdai hozzáféréssel rendelkezik, a helyreállítási kulcsot (Jelszó) a következő parancs rendszergazdai jogú parancssorból való futtatásával láthatja:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Ha az eszközt az Intune-ban való regisztráció előtt titkosították, előfordulhat, hogy a helyreállítási kulcsot az OOBE-folyamat során az eszközbe való bejelentkezéshez használt "Microsoft-fiók" (MSA) társította. Ebben az esetben az MSA elérésének és az azzal való bejelentkezésnek meg kell mutatnia az eszközöket, amelyek helyreállítási kulcsait  https://onedrive.live.com/recoverykey tárolta.
 
Ha az eszközt tartományalapú csoportházirenden keresztül konfigurálva titkosította, a helyreállítási információkat a rendszer a számítógép active directoryjában tárolhatja.

Ha konfigurálta az Végpontvédelmi házirendet a helyreállítási kulcs Azure Active Directory-ban való tárolására, de egy adott eszköz kulcsát még nem töltötte fel, a feltöltést úgy elindíthatja, hogy a mem konzolról elforgatja az adott eszköz helyreállítási kulcsát. A részletekért [lásd: BitLocker helyreállítási kulcsok elforgatása.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

