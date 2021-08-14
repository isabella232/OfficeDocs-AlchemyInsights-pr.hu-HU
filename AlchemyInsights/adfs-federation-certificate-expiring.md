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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952971"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS összevonási tanúsítvány lejárata

A probléma megoldásához kövesse az alábbi lépéseket:
  
1. Telepítse Microsoft Azure Active Directory modul Windows PowerShell számítógépen (ha a modul még nincs telepítve). Ehhez a Manage [Azure AD using Windows PowerShell (Azure AD](https://aka.ms/aadposh)kezelése a Windows PowerShell.

2. Kövesse "1. forgatókönyv: Az AD FS jogkivonat-aláíró tanúsítvány lejárt" szakaszának "Hiba történt a webhely elérésében" hibaüzenetet az AD FS szolgáltatásból, amikor egy összevont felhasználó bejelentkezik az [Microsoft 365-be,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)az Azure-ba vagy az Intune-ba.

3. Kövesse az Összevont tartomány beállításainak frissítése vagy javítása a Microsoftban, az Azure-ban vagy az [Intune-ban található lépéseket.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Az összevonási tanúsítványok megújítását az Összevonási tanúsítványok megújítása az összevonási és összevonási Microsoft 365 [és Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
