---
title: Az egyik helyszíni összevonási szolgáltatási tanúsítvány lejár
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673499"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Az egyik helyszíni összevonási szolgáltatási tanúsítvány lejár

A probléma megoldásához kövesse az alábbi lépéseket:
  
- Telepítse a Windows PowerShellhez készült Microsoft Azure Active Directory modult a számítógépen (ha még nincs telepítve a modul). Ehhez nyissa meg az [Azure Active Directory PowerShellt a Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) -hoz.
    
- Kövesse a következő témakörben szereplő lépéseket: az AD FS-jogkivonat-aláíró tanúsítvány lejárt "az [" nem sikerült elérni a webhelyet "hibaüzenet jelenik meg az AD FS-ből, ha egy szövetséges felhasználó bejelentkezik a Microsoft 365, Azure vagy Intune szolgáltatásba](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Kövesse a következő témakör lépéseit: a [Microsoft 365, Azure vagy Intune rendszerbeli összevont tartományok beállításainak frissítése vagy kijavítása](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Az összevonási tanúsítványok megújításáról további információt a [tanúsítvány megújítása a O365 és az Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)szolgáltatáshoz című témakörben talál.
  

