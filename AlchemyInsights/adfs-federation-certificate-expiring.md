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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="18274-102">Az ADFS összevonási tanúsítvány lejárata</span><span class="sxs-lookup"><span data-stu-id="18274-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="18274-103">A probléma megoldásához hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="18274-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="18274-104">Telepítse a Microsoft Azure Active Directory module for Windows PowerShell a számítógépre (ha a modul még nincs telepítve).</span><span class="sxs-lookup"><span data-stu-id="18274-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="18274-105">Ehhez nyissa meg [az Azure AD kezelése a Windows PowerShell használatával](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="18274-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="18274-106">Kövesse az AD FS "Az AD FS-jogkivonat-aláíró tanúsítvány lejárta" című szakaszának "Hiba volt a webhely elérése" című szakaszának [lépéseit, amikor egy összevont felhasználó bejelentkezik a Microsoft 365, az Azure vagy az Intune rendszerbe.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="18274-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="18274-107">Kövesse az [összevont tartomány frissítésével vagy javításával a Microsoft, az Azure vagy az Intune beállításainak frissítése vagy javítása című lépéseit.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="18274-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="18274-108">Az összevonási tanúsítványok megújításáról a [Microsoft 365 és az Azure Active Directory összevonási tanúsítványok megújítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="18274-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
