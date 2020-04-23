---
title: Jelszó-szinkronizálás – problémamegoldás
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732512"
---
# <a name="troubleshoot-password-synchronization"></a>Jelszó-szinkronizálás – problémamegoldás

Olyan problémák elhárítása, amelyek miatt nincsenek jelszavak szinkronizálása az Azure AD Connect 1.1.614.0-s vagy újabb verziójával:
  
1. Nyisson meg egy új Windows PowerShell-munkamenetet az Azure AD Connect kiszolgálón a **Futtatás rendszergazdaként** beállítással.

2. Futtassa **a Set-ExecutionPolicy RemoteSigned** vagy **Set-ExecutionPolicy Unrestricted (Set-ExecutionPolicy ) futtatása korlátozás nélkül.**

3. Indítsa el az Azure AD Connect varázslót.

4. Nyissa meg a **További feladatok** lapot, válassza **a Hibaelhárítás**lehetőséget, és kattintson a **Tovább**gombra.

5. A Hibaelhárítás lapon kattintson az Indítás gombra a PowerShell hibaelhárítási menüjének **elindításához.**

6. A főmenüben válassza a **Jelszó-szinkronizálás hibaelhárítása lehetőséget.**

7. Az almenüben válassza a **Jelszó-szinkronizálás parancs átnem nem működik.**

**A hibaelhárítási feladat eredményeinek megismerése**
  
A hibaelhárítási feladat a következő ellenőrzéseket hajtja végre:
  
- Ellenőrzi, hogy a jelszó-szinkronizálási funkció engedélyezve van-e az Azure AD-bérlőhöz.

- Ellenőrzi, hogy az Azure AD Connect-kiszolgáló nincs-e átmeneti módban.

- Minden meglévő helyszíni Active Directory-összekötő esetén (amely egy meglévő Active Directory-erdőnek felel meg):

- 
  - Ellenőrzi, hogy a jelszó-szinkronizálási szolgáltatás engedélyezve van-e.

  - Jelszó-szinkronizálási szívverési események keresése a Windows alkalmazás eseménynaplóiban.

  - A helyszíni Active Directory-összekötő alatti minden Egyes Active Directory-tartomány esetén:

  - Ellenőrzi, hogy a tartomány elérhető-e az Azure AD Connect-kiszolgálóról.

  - Ellenőrzi, hogy a helyszíni Active Directory-összekötő által használt Active Directory tartományi szolgáltatások (AD DS) fiókok rendelkeznek-e a jelszó-szinkronizáláshoz szükséges megfelelő felhasználónévvel, jelszóval és engedélyekkel.

A jelszószinkronizálás hibaelhárításával kapcsolatos további segítségért olvassa el a [Jelszó-szinkronizálás hibaelhárítása az Azure AD Connect szinkronizálásával című témakört.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)
  