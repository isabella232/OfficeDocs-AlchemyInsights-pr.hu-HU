---
title: ADFS összevonási tanúsítvány ennyi időn belül lejár
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293496"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS összevonási tanúsítvány ennyi időn belül lejár

A probléma megoldásához kövesse az alábbi lépéseket:
  
1. A Microsoft Azure Active Directory modult a Windows PowerShell telepítése a számítógépen (Ha a modul nincs még telepítve). Ehhez lépjen [kezelése a Windows PowerShell Azure AD](https://aka.ms/aadposh).
    
2. Kövesse az "1. eset: az AD FS-jogkivonat-aláíró tanúsítvány lejárt" részében a ["Hiba történt a webhely eléréséhez" hiba az Active Directory összevonási szolgáltatások összevont felhasználó bejelentkezik az Office 365, Azure, vagy Intune esetén](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Kövesse a [frissítés, vagy a beállításokat az Office 365, Azure, vagy Intune összevont tartomány javítása](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    További információ összevonási ismerhet [Office 365 és Azure az Active Directory összevonási tanúsítványok megújítása](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben talál.
    

