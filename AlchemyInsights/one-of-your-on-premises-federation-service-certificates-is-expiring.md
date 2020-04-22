---
title: Az egyik helyszíni összevonási szolgáltatástanúsítvány lejár
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761385"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Az egyik helyszíni összevonási szolgáltatástanúsítvány lejár

A probléma megoldásához hajtsa végre az alábbi lépéseket:
  
- Telepítse a Microsoft Azure Active Directory module for Windows PowerShell a számítógépre (ha a modul még nincs telepítve). Ehhez nyissa meg az [Azure Active Directory PowerShell for Graph-ot.](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Kövesse az AD FS "Az AD FS-jogkivonat-aláíró tanúsítvány lejárta" című szakaszának ["Hiba történt a webhely elérése közben" című hiba "Hiba történt a webhely elérése közben" című hiba lépéseit, amikor egy összevont felhasználó bejelentkezik az Office 365-be, az Azure-ba vagy az Intune-ba.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Kövesse a[t. T. Összevont tartomány beállításainak frissítése vagy javítása az Office 365-ben, az Azure-ban vagy az Intune-ban](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)című t.
    
Az összevonási tanúsítványok megújításáról az [O365 és az Azure AD tanúsítványmegújítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben talál további információt.
  

