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
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810054"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="00b44-102">A helyszíni összevonási szolgáltatási tanúsítványok egyike hamarosan lejár</span><span class="sxs-lookup"><span data-stu-id="00b44-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="00b44-103">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="00b44-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="00b44-104">Telepítse a Microsoft Azure Active Directory modult a Windows PowerShellhez a számítógépen (ha a modul még nincs telepítve).</span><span class="sxs-lookup"><span data-stu-id="00b44-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="00b44-105">Ehhez a következőt kell látnia: [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="00b44-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="00b44-106">Kövesse "1. forgatókönyv: Az AD FS-jogkivonat lejárt" című szakasz "Hiba történt a webhely elérésében" című szakasz lépéseit, amikor egy összevont felhasználó bejelentkezik [a Microsoft 365-be,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)az Azure-ba vagy az Intune-ba.</span><span class="sxs-lookup"><span data-stu-id="00b44-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="00b44-107">Kövesse az Összevont tartomány beállításainak frissítése vagy javítása [a Microsoft 365-ben,](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)az Azure-ban vagy az Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="00b44-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="00b44-108">Az összevonási tanúsítványok megújításáról további információt A tanúsítvány megújítása az O365-ről és az [Azure AD-ről.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="00b44-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

