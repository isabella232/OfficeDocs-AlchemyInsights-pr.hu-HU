---
title: Az ADFS-összevonási tanúsítvány lejárata
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686716"
---
# <a name="adfs-federation-certificate-expiring"></a>Az ADFS-összevonási tanúsítvány lejárata

A probléma megoldásához kövesse az alábbi lépéseket:
  
1. Telepítse a Windows PowerShellhez készült Microsoft Azure Active Directory modult a számítógépen (ha még nincs telepítve a modul). Ehhez nyissa meg az [Azure ad kezelése a Windows PowerShell használatával](https://aka.ms/aadposh)című cikk lépéseit.

2. Kövesse a következő témakörben szereplő lépéseket: az AD FS-jogkivonat-aláíró tanúsítvány lejárt "az [" nem sikerült elérni a webhelyet "hibaüzenet jelenik meg az AD FS-ből, ha egy szövetséges felhasználó bejelentkezik a Microsoft 365, Azure vagy Intune szolgáltatásba](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Kövesse a következő témakör lépéseit: az [összevont tartományok frissítése vagy javítása a Microsoft, Azure vagy Intune környezetben](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Ha többet szeretne tudni az összevonási tanúsítványok megújításáról, olvassa el [az összevonási tanúsítványok megújítása a Microsoft 365 és az Azure Active Directory szolgáltatásban](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakört.
