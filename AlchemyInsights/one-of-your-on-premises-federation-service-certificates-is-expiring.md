---
title: A helyszíni összevonási szolgáltatási tanúsítványok egyike hamarosan lejár
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985219"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>A helyszíni összevonási szolgáltatási tanúsítványok egyike hamarosan lejár

A probléma megoldásához kövesse az alábbi lépéseket:
  
- Telepítse Microsoft Azure Active Directory modul Windows PowerShell számítógépen (ha a modul még nincs telepítve). Ehhez a Azure Active Directory [PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Kövesse "1. forgatókönyv: Az AD FS jogkivonat-aláíró tanúsítvány lejárt" szakaszának "Hiba történt a webhely elérésében" hibaüzenetet az AD FS szolgáltatásból, amikor egy összevont felhasználó bejelentkezik az [Microsoft 365-be,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)az Azure-ba vagy az Intune-ba.
    
- Kövesse az Összevont tartomány beállításainak frissítése vagy javítása az Microsoft 365, az Azure-ban vagy az [Intune-ban Microsoft 365 lépéseket.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Az összevonási tanúsítványok megújításáról további információt A tanúsítvány megújítása az O365-ről és az [Azure AD-ről.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

