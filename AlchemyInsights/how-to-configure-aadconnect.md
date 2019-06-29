---
title: 646 hogyan kell beállítani a AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385346"
---
# <a name="configure-sync-features"></a>Szinkronizálási szolgáltatás konfigurálása

Azure AD csatlakozás tartalmaz számos szolgáltatása alapértelmezés szerint engedélyezve vannak, vagy később is engedélyezheti. Egyes szolgáltatások igényel további konfigurálást adott környezetben.

- Az objektumok [szűrése](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) korlátok Azure AD a rendszer szinkronizálja. Alapértelmezés szerint minden felhasználók, kapcsolatok, csoportok, és a Windows 10 számítógépfiókot szinkronizálódnak. Akkor figyelembe vehetjük vagy kihagyhatjuk objektumok tartományok, szervezeti egységek és más jellemzők alapján.

- [Kivonat jelszó-szinkronizálás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) a jelszó kivonatértékét az Active Directory címtárból helyszíni Azure ad szinkronizálja. Ez lehetővé teszi a jelszavak kezelését egy helyről, de ugyanazt a jelszót mindkét helyszíni és cloud környezetekben. Mivel az Active Directory a mérvadó információforrás, használhatja a saját jelszóházirendek.

- [Az önkiszolgáló jelszó alaphelyzetbe állítása (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) lehetővé teszi a felhasználók alaphelyzetbe saját jelszavukat a felhőben továbbra is az a helyi jelszóházirend alkalmazása közben.

- [Eszköz visszaírása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lehetővé teszi a regisztrált Azure Active Directory írják vissza a helyszíni Active Directory, a feltételes hozzáférésre használható.

- [Véletlen rlés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) alapértelmezés szerint engedélyezve van túl sok egyidejű objektum törlése (500-nál több objektumot szinkronizálás) elkerülése érdekében. Ez a beállítás a vállalata igényeinek megfelelően módosíthatja.

- Expressz telepítés esetén alapértelmezés szerint engedélyezett [az automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) , és így biztosítható a Azure AD csatlakozás verziója mindig aktuális.
