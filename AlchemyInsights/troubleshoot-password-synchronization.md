---
title: Jelszó-szinkronizálás hibaelhárítása
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664928"
---
# <a name="troubleshoot-password-synchronization"></a>Jelszó-szinkronizálás hibaelhárítása

A jelszó-szinkronizálási hibák elhárításához Kezdje a AAD csatlakoztatása hibaelhárítási feladattal annak megállapításához, hogy miért nem szinkronizálja a jelszavakat. A kezdéshez lépjen a [közvetlen szinkronizálás kezelése](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)elemre.  

1. Nyisson meg egy új Windows PowerShell-munkamenetet az Azure AD Connect-kiszolgálón, és válassza a **Futtatás rendszergazdaként** lehetőséget.

2. Futtassa a Set-ExecutionPolicy RemoteSigned vagy a Set-ExecutionPolicy korlátozás nélküli beállítást.

3. Indítsa el az Azure AD Connect varázslót.

4. Lépjen a további feladatok lapra > **Hibaelhárítás**című témakört  >  **Next**.

5. Válassza az **Indítás** gombot a PowerShell hibaelhárítási menüjének megnyitásához.

6. Válassza a **Jelszó-szinkronizálás elhárítása**lehetőséget.

    A probléma általában az, hogy egy adott felhasználói fiókhoz nincs szinkronizálva jelszó.

    **Megjegyzések** A jelszó-szinkronizálás sikertelen, ha az utolsó sikeres jelszó-szinkronizálás néhány évvel ezelőtt volt.

A jelszó-szinkronizálással kapcsolatos további segítségért olvassa el a [jelszó-ujjlenyomat szinkronizálása az Azure ad Connect szinkronizálásával](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)című témakört.