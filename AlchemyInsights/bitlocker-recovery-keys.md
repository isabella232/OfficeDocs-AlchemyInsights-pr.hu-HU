---
title: BitLocker helyreállítási kulcsok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685888"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Hozzáférés a BitLocker helyreállítási kulcsaihoz

A BitLocker-beállítások Intune-végpontok védelmi házirendjének konfigurálásakor meghatározhatja, hogy a BitLocker helyreállítási információkat az Azure Active Directoryban kell-e tárolni.

Ha ez a beállítás be van állítva, akkor a tárolt helyreállítási adatoknak a Intune-rendszergazdák számára kétféleképpen kell szerepelniük az Intune-eszközök lapon, a következő két módon:

Eszközök – Azure AD-eszközök – > "eszköz" vagy eszközök – > minden eszköz – > "eszköz" – > helyreállítási kulcsok

Azt is megteheti, hogy az eszközhöz rendszergazdai hozzáférés van megnyitva, a helyreállítási kulcs (jelszó) a következő parancs futtatásával tekinthető meg egy rendszergazdai jogú parancssorból:

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
Ha az eszköz az Intune-ba való bejelentkezés előtt titkosított, lehet, hogy a helyreállítási kulcs társítva van a Microsoft-fiókhoz (MSA), amellyel az OOBE folyamat során bejelentkezhet az eszközre. Ebben az esetben a MSA való hozzáférés  https://onedrive.live.com/recoverykey és bejelentkezés során meg kell jeleníteni azokat az eszközöket, amelyekhez a helyreállítási kulcsokat tárolták.
 
Ha az eszköz tartományon alapuló csoportházirend-konfiguráción keresztül volt titkosítva, a helyreállítási adatok a helyszíni Active Directoryban tárolhatók.
 

