---
title: 646 Az AADConnect konfigurálása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722561"
---
# <a name="configure-sync-features"></a>Szinkronizálási szolgáltatások konfigurálása

Az Azure AD Connect számos olyan funkciót tartalmaz, amelyek alapértelmezés szerint engedélyezve vannak, vagy amelyeket később engedélyezhet. Egyes szolgáltatások további konfigurációt igényelnek bizonyos környezetekben.

- [A szűrés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) korlátozza az objektumok szinkronizálását az Azure AD-vel. Alapértelmezés szerint a rendszer minden felhasználót, kapcsolattartót, csoportot és Windows 10-es számítógépfiókot szinkronizál. Tartományon, ous-okon vagy más attribútumokon alapuló objektumokat is felvehet vagy kizárhat.

- [A jelszókivonat-szinkronizálás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) szinkronizálja a jelszókivonatot a helyszíni Active Directoryból az Azure AD-be. Ez lehetővé teszi a jelszókezelést egy helyen, de ugyanazt a jelszót használja mind a helyszíni, mind a felhőalapú környezetekben. Mivel az Active Directory a mérvadó forrás, használhatja a saját jelszóházirendeket.

- [Az önkiszolgáló jelszó-visszaállítás (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) lehetővé teszi a felhasználók számára, hogy alaphelyzetbe állítsák saját jelszavukat a felhőben, miközben továbbra is alkalmazzák a helyszíni jelszóházirendet.

- [Az eszközvisszaírás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lehetővé teszi, hogy az Azure AD-ben regisztrált eszközök visszaírhatók legyenek a helyszíni Active Directoryba, így feltételes hozzáféréshez használhatók.

- [A véletlen törlés megakadályozása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) alapértelmezés szerint engedélyezve van a túl sok egyidejű objektumtörlés megakadályozása érdekében (szinkronizálásonként több mint 500 objektum). Ezt a beállítást a szervezet igényeinek megfelelően módosíthatja.

- [Az automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) alapértelmezés szerint engedélyezve van az expressz telepítésekhez, és biztosítja, hogy az Azure AD Connect verziója mindig aktuális legyen.
