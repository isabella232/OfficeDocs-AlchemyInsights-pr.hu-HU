---
title: Jelszó-szinkronizálás – problémamegoldás
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387879"
---
# <a name="troubleshoot-password-synchronization"></a>Jelszó-szinkronizálás – problémamegoldás

A jelszó-szinkronizálási problémák elhárításához először használja ezt az AAD Connect hibaelhárítási feladatot annak megállapítására, hogy miért nem szinkronizálják a jelszavakat. A kezdéshez nyissa meg [a Közvetlen szinkronizálás kezelése](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)című.  

1. Nyisson meg egy új Windows PowerShell-munkamenetet az Azure AD Connect-kiszolgálón, és válassza a **Futtatás rendszergazdaként** lehetőséget.

2. Futtassa a Set-ExecutionPolicy RemoteSigned vagy Set-ExecutionPolicy Unrestricted (Set-ExecutionPolicy) futtatása korlátozás nélkül.

3. Indítsa el az Azure AD Connect varázslót.

4. Nyissa meg a További feladatok lapot > **Következő hibaelhárítást.**  >  **Next**

5. Válassza az **Indítás** lehetőséget a PowerShell hibaelhárítási menüjének megnyitásához.

6. Válassza a **Jelszó-szinkronizálás hibaelhárítása lehetőséget.**

    A probléma általában az, hogy a jelszó nincs szinkronizálva egy adott felhasználói fiókhoz.

    **Megjegyzések** A jelszószinkronizálás sikertelen, ha az utolsó sikeres jelszószinkronizálás néhány évvel ezelőtt volt.

A jelszó-szinkronizálás hibaelhárításával kapcsolatos további segítségért olvassa el [A jelszókivonat-szinkronizálás hibaelhárítása az Azure AD Connect szinkronizálásával című témakört.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)