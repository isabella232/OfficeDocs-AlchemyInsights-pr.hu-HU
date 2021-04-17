---
title: ADFS összevonási tanúsítvány lejárata
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
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821953"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS összevonási tanúsítvány lejárata

A probléma megoldásához kövesse az alábbi lépéseket:
  
1. Telepítse a Microsoft Azure Active Directory modult a Windows PowerShellhez a számítógépen (ha a modul még nincs telepítve). Ehhez az Azure AD kezelése a Windows PowerShell használatával 2010-et [kell használnia.](https://aka.ms/aadposh)

2. Kövesse "1. forgatókönyv: Az AD FS-jogkivonat lejárt" című szakasz "Hiba történt a webhely elérésében" című szakasz lépéseit, amikor egy összevont felhasználó bejelentkezik [a Microsoft 365-be,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)az Azure-ba vagy az Intune-ba.

3. Kövesse az Összevont tartomány beállításainak frissítése vagy javítása a Microsoftban, az Azure-ban vagy az [Intune-ban található lépéseket.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Az összevonási tanúsítványok megújítását A [Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)és az Azure Active Directory összevonási tanúsítványának megújításacímú cikk mutatja be.
