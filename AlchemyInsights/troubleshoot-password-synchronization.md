---
title: A jelszó-szinkronizálás hibaelhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767178"
---
# <a name="troubleshoot-password-synchronization"></a>A jelszó-szinkronizálás hibaelhárítása

Nincs jelszó esetén szinkronizált Azure AD csatlakozás verziója 1.1.614.0 vagy annál újabb problémák elhárításához:
  
1. Nyissa meg a Azure AD csatlakozás kiszolgálón egy új Windows PowerShell munkamenetet a **Futtatás rendszergazdaként** beállítással. 
    
2. Futtassa a **Set-ExecutionPolicy RemoteSigned** vagy a **Set-ExecutionPolicy korlátlan**. 
    
3. Borzas AD csatlakozás varázsló elindításához.
    
4. Keresse meg a ** további feladatok ** lapon adja ** elhárítása **, és kattintson a **Tovább**gombra. 
    
5. A hibaelhárítás lapon kattintson **a hibaelhárítás mikéntje az indítási** menü a PowerShell. 
    
6. Válassza a főmenü, **A jelszó-szinkronizálás hibaelhárítása**. 
    
7. Válassza ki a sub menü **Jelszó-szinkronizálás egyáltalán nem működik**. 
    
 **A hibaelhárítási feladat az eredmények értelmezésében**
  
A hibaelhárítási feladat a következő ellenőrzéseket hajtja végre:
  
- Ellenőrzi, hogy a jelszó-szinkronizálás szolgáltatás engedélyezve van a Azure AD bérlő.
    
- Ellenőrzi, hogy a Borzas AD csatlakozás kiszolgáló nincs a fejlesztői üzemmód.
    
- Minden meglévő helyszíni Active Directory Connector (amely megfelel a meglévő Active Directory-erdő):
    
- 
  - Ellenőrzi, hogy a jelszó-szinkronizálás szolgáltatás engedélyezve van.
    
  - Jelszó szinkronizálás szívverés események a Windows alkalmazás-eseménynaplókban keres.
    
  - Minden egyes Active Directory tartomány alapján a helyszíni Active Directory-csatoló:
    
  - Ellenőrzi, hogy a tartomány a Azure AD csatlakozás kiszolgálóról érhető.
    
  - Ellenőrzi, hogy a helyszíni Active Directory-csatolója az Active Directory tartományi szolgáltatások (AD DS) fiókokat rendelkezik-e a helyes felhasználónév, jelszó és a jelszó-szinkronizálás szükséges engedélyek.
    
Jelszó-szinkronizálás hibáinak elhárítása További segítséget talál [Azure AD csatlakozás szinkronizálás a jelszó-szinkronizálás hibaelhárítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

