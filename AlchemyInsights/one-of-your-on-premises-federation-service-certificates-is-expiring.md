---
title: A helyi összevonási szolgáltatás tanúsítványok közül van lejáró
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473322"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>A helyi összevonási szolgáltatás tanúsítványok közül van lejáró

A probléma megoldásához kövesse az alábbi lépéseket:
  
- A Microsoft Azure Active Directory modult a Windows PowerShell telepítése a számítógépen (Ha a modul nincs még telepítve). Ehhez nyissa meg a [Grafikon Azure Active Directory PowerShell](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Kövesse az "1. eset: az AD FS-jogkivonat-aláíró tanúsítvány lejárt" részében a ["Hiba történt a webhely eléréséhez" hiba az Active Directory összevonási szolgáltatások összevont felhasználó bejelentkezik az Office 365, Azure, vagy Intune esetén](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Kövesse t[frissíteni, vagy a beállításokat az Office 365, Azure, vagy Intune összevont tartomány javítása](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Összevonási tanúsítványok megújításával kapcsolatos további tudnivalókért lásd: [tanúsítvány-megújítási O365 és Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

