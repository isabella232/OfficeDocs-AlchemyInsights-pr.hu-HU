---
title: BitLocker helyreállítási kulcsok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908817"
---
# <a name="accessing-bitlocker-recovery-keys"></a>A BitLocker helyreállítási kulcsainak elérése

Amikor beállítja a BitLocker-beállításokat, a végponti védelmi házirendet, meg lehet határozni, hogy a BitLocker helyreállítási információit a Azure Active Directory szolgáltatásban kell-e tárolni.

Ha ez a beállítás be van állítva, akkor a tárolt helyreállítási adatoknak láthatónak kell lenniük az adott eszköz rekordjának az Intune eszközök lapátja alatt az eszközbejegyzés adatainak részeként kétféle módon:

Készülékek-Azure AD eszközök-> "eszköz" vagy eszközök-> minden eszköz-> "Device"-> helyreállítási kulcsok

Vagylagosan, ha van közigazgatási belépés-hoz berendezés maga, a visszaszerzés kulcs (jelszó) lehet látott mellett futás a következő követel-ból egy emelkedett követel gyors:

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
Ha az eszköz az Intune-be történő beiratkozás előtt lett titkosítva, akkor lehet, hogy a helyreállítási kulcs hozzá van rendelve a "Microsoft fiók" (MSA) eszközhöz, amellyel az OOBE folyamat során bejelentkezik az eszközre. Ha ez volt a helyzet, bejutó https://onedrive.live.com/recoverykey és jel-ban-val amit MSA kellet volna mutat a berendezés részére melyik visszaszerzés kulcsok voltak raktározott.
 
Ha az eszköz a tartomány alapú csoportházirenddel történő konfigurálás eredményeképpen lett titkosítva, a helyreállítási adatok a helyszíni Active Directoryban tárolhatók.
 

