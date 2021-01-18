---
title: Probléma a virtuális gépekhez való csatlakozásnál
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885209"
---
# <a name="issue-joining-vms"></a>Probléma a virtuális gépekhez való csatlakozásnál

A következő lépésekkel oldhatja meg a virtuális gépekhez való csatlakozáskor előforduló problémákat:

1. Próbáljon meg **upn** formátumban (például "joeuser@contoso.com") bejelentkezni a **SAMAccountName** formátum ('CONTOSO\jojauser') helyett.
2. Győződjön meg arról, hogy az első lépéseket  követve engedélyezte a jelszó-szinkronizálást.
3. Győződjön meg arról, hogy az érintett felhasználói fiók nem külső fiók az Azure AD bérlői webhelyen. A külső felhasználók nem tudnak bejelentkezni a felügyelt tartományba, mert az Azure AD tartományi szolgáltatások nem tartalmaznak hitelesítő adatokat az ilyen felhasználói fiókokhoz.
4. Ha az érintett felhasználói fiók csak felhőalapú felhasználói fiók, győződjön meg arról, hogy a felhasználók megváltoztatták a jelszavukat az Azure AD tartományi szolgáltatások engedélyezése után. Ez a lépés az Azure AD tartományi szolgáltatások generálása érdekében szükséges hitelesítő adatokhoz szükséges hitelesítő adatokat generálja.
5. Ha az érintett felhasználói fiókok szinkronizálva vannak egy helyszíni címtárból, ellenőrizze, hogy az Azure AD Connect ajánlott kiadása be van-e állítva teljes szinkronizálásra.
6. Ha a 4. lépés megerősítése után a problémák továbbra is fennállnak, hajtsa végre a következő parancsokat a szinkronizálási gépről:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.