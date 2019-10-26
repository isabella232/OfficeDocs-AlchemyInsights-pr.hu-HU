---
title: Az ADFS összevonási tanúsítványának lejárása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737191"
---
# <a name="adfs-federation-certificate-expiring"></a>Az ADFS összevonási tanúsítványának lejárása

A probléma megoldásához hajtsa végre az alábbi lépéseket:
  
1. A Microsoft Azure Active Directory-modul telepítése a számítógépre a Windows PowerShell környezethez (ha a modul még nincs telepítve). Ehhez nyissa meg a [Windows PowerShell eszközzel a Azure rendszer kezelését](https://aka.ms/aadposh).

2. Kövesse a "1. forgatókönyv: az Active Directory összevonási szolgáltatások jogkivonat-aláíró tanúsítványa lejárt" című szakaszt "a [hely elérésekor hiba történt" hibaüzenet, amikor egy szövetséges felhasználó bejelentkezik az Office 365, Azure vagy Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)szolgáltatásba,

3. Kövesse a frissítés lépéseit, [vagy javítsa az összevont tartomány beállításait az Office 365, Azure vagy Intune tartományban](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    További információt az összevonási tanúsítványok megújításáról [az Office 365 és a Azure Active Directory összevonási tanúsítványainak megújítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben talál.
