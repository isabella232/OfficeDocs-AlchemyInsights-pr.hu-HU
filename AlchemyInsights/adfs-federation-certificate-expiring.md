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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="ab44a-102">ADFS összevonási tanúsítvány lejárata</span><span class="sxs-lookup"><span data-stu-id="ab44a-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="ab44a-103">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="ab44a-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="ab44a-104">Telepítse a Microsoft Azure Active Directory modult a Windows PowerShellhez a számítógépen (ha a modul még nincs telepítve).</span><span class="sxs-lookup"><span data-stu-id="ab44a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="ab44a-105">Ehhez az Azure AD kezelése a Windows PowerShell használatával 2010-et [kell használnia.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="ab44a-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="ab44a-106">Kövesse "1. forgatókönyv: Az AD FS-jogkivonat lejárt" című szakasz "Hiba történt a webhely elérésében" című szakasz lépéseit, amikor egy összevont felhasználó bejelentkezik [a Microsoft 365-be,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)az Azure-ba vagy az Intune-ba.</span><span class="sxs-lookup"><span data-stu-id="ab44a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="ab44a-107">Kövesse az Összevont tartomány beállításainak frissítése vagy javítása a Microsoftban, az Azure-ban vagy az [Intune-ban található lépéseket.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="ab44a-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="ab44a-108">Az összevonási tanúsítványok megújítását A [Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)és az Azure Active Directory összevonási tanúsítványának megújításacímú cikk mutatja be.</span><span class="sxs-lookup"><span data-stu-id="ab44a-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
