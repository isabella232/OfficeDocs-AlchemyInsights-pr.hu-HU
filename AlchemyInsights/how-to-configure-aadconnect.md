---
title: 646 Az AADConnect konfigurálása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963645"
---
# <a name="configure-sync-features"></a>Szinkronizálási szolgáltatások konfigurálása

Az Azure AD Csatlakozás szolgáltatás számos, alapértelmezés szerint engedélyezett, illetve később engedélyezhető szolgáltatást tartalmaz. Egyes funkciókhoz további beállításokat kell konfigurálni az adott környezetben.

- [Szűrési](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) korlátozások: Az objektumok szinkronizálódnak az Azure AD szolgáltatásba. Alapértelmezés szerint a rendszer minden felhasználót, névjegyet, csoportot és Windows 10 számítógépfiókot. Tartományon, OUson vagy más attribútumon alapuló objektumokat is tartalmazhat, illetve kizárhat.

- [A jelszó kivonat-szinkronizálása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) szinkronizálja a jelszó kivonatát a helyszíni Active Directoryból az Azure AD-be. Ez lehetővé teszi a jelszókezelést egy helyen, de ugyanazt a jelszót használja helyszíni és felhőbeli környezetekben is. Mivel az Active Directory a mérvadó forrás, saját jelszóházira vonatkozó házirendeket is használhat.

- [Az önkiszolgáló](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) jelszó-visszaállítással a felhasználók a helyszíni jelszó-házirend alkalmazása mellett alaphelyzetbe állíthatják a jelszavukat a felhőben.

- [Az eszközvisszaírással](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) a regisztrált eszközök az Azure AD-ban visszaírhatóak a helyszíni Active Directoryba, így feltételes hozzáférésre használhatók.

- [A véletlen törlések](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) megakadályozása alapértelmezés szerint engedélyezve van, hogy megakadályozza a túl sok egyidejű objektumtörlést (szinkronizálásonként több mint 500 objektumot). Ezt a beállítást a szervezete igényeinek megfelelően módosíthatja.

- [Az automatikus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) frissítés alapértelmezés szerint engedélyezve van a gyors telepítések esetén, és segít abban, hogy az Azure AD-Csatlakozás mindig aktuális legyen.
