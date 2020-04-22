---
title: Az ADFS összevonási tanúsítvány lejárata
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
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710409"
---
# <a name="adfs-federation-certificate-expiring"></a>Az ADFS összevonási tanúsítvány lejárata

A probléma megoldásához hajtsa végre az alábbi lépéseket:
  
1. Telepítse a Microsoft Azure Active Directory module for Windows PowerShell a számítógépre (ha a modul még nincs telepítve). Ehhez nyissa meg [az Azure AD kezelése a Windows PowerShell használatával](https://aka.ms/aadposh).

2. Kövesse az AD FS "Az AD FS-jogkivonat-aláíró tanúsítvány lejárta" című szakaszának "Hiba volt a webhely elérése" című szakaszának [lépéseit, amikor egy összevont felhasználó bejelentkezik a Microsoft 365, az Azure vagy az Intune rendszerbe.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Kövesse az [összevont tartomány frissítésével vagy javításával a Microsoft, az Azure vagy az Intune beállításainak frissítése vagy javítása című lépéseit.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Az összevonási tanúsítványok megújításáról a [Microsoft 365 és az Azure Active Directory összevonási tanúsítványok megújítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben olvashat bővebben.
