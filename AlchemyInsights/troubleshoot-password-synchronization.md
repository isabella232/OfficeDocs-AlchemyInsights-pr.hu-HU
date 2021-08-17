---
title: Jelszó-szinkronizálási hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105753"
---
# <a name="troubleshoot-password-synchronization"></a>Jelszó-szinkronizálási hibák elhárítása

A jelszavak szinkronizálásával kapcsolatos hibák elhárításához használja ezt az AAD-Csatlakozás, és állapítsa meg, hogy miért nem szinkronizálódnak a jelszavak. Első nekikezdhet a Közvetlen [szinkronizálás kezelése ásban.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Nyisson meg egy Windows PowerShell az Azure AD Csatlakozás-kiszolgálón, és válassza a Futtatás **rendszergazdaként** lehetőséget.

2. Futtassa Set-ExecutionPolicy RemoteSigned vagy Set-ExecutionPolicy unrestricted.

3. Indítsa el az Azure AD Csatlakozás varázslót.

4. A További feladatok lapra lépéshez > **Következő**  >  **hibaelhárítása gombra.**

5. Válassza **az Indítás** elemet a PowerShell hibaelhárítási menüjének megnyitásához.

6. Válassza **a Jelszó-szinkronizálási hibák elhárítása lehetőséget.**

    A probléma általában az, hogy egy adott felhasználói fiók jelszava nincs szinkronizálva.

    **Megjegyzések** A jelszószinkronizálás nem sikerül, ha a legutóbbi sikeres jelszó-szinkronizálás már jó ideje történt.

A jelszószinkronizálással kapcsolatos további segítségért lásd: Jelszó kivonat-szinkronizálási hibák elhárítása [az Azure AD Csatlakozás használatával.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)