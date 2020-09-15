---
title: a 646 beállítása a AADConnect
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704491"
---
# <a name="configure-sync-features"></a>Szinkronizálási szolgáltatások beállítása

Az Azure AD Connect alapértelmezés szerint számos olyan funkciót tartalmaz, amely alapértelmezés szerint engedélyezve van, vagy később is engedélyezhető. Egyes funkciókhoz további beállításokra van szükség bizonyos környezetekben.

- [Szűrés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) : az objektumok szinkronizálása az Azure ad szolgáltatással történik. Alapértelmezés szerint minden felhasználó, névjegy, csoport és Windows 10 számítógépfiók szinkronizálva van. Az objektumokat tartományok, szervezeti egységek vagy egyéb attribútumok alapján is megadhatja vagy kihagyhatja.

- A [jelszó-ujjlenyomat szinkronizálása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) szinkronizálja a jelszó-ujjlenyomatot a helyszíni Active Directoryból az Azure ad szolgáltatásba. Ez lehetővé teszi a jelszavak kezelését egyetlen helyen, de ugyanazt a jelszót használja mind a helyszíni, mind a Felhőbeli környezetekben. Mivel az Active Directory a mérvadó forrás, használhatja saját jelszavas házirendjeit.

- Önkiszolgáló [jelszó-visszaállító (Visszaállítás)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) : lehetővé teszi a felhasználóknak, hogy alaphelyzetbe állítsanak saját jelszavait a felhőben, miközben továbbra is alkalmazzák a helyszíni jelszavas házirendet.

- Az [eszköz writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lehetővé teszi, hogy az Azure ad-beli regisztrált eszközök visszalegyenek a helyszíni Active Directoryhoz, így felhasználhatók feltételes hozzáférésre.

- A [véletlen törlések megelőzése](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) alapértelmezés szerint engedélyezve van, hogy ne legyenek túl sok egyidejű objektum törlése (több mint 500 objektum/szinkronizálás esetén). Ezt a beállítást a szervezet igényeinek megfelelően változtathatja meg.

- Az [automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) alapértelmezés szerint engedélyezve van az Express-telepítésekben, és biztosítja, hogy az Azure ad Connect verziója mindig naprakész legyen.
