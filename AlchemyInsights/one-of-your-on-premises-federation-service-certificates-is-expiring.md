---
title: Az egyik helyszíni összevonási szolgáltatástanúsítvány lejár
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761385"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="d09f8-102">Az egyik helyszíni összevonási szolgáltatástanúsítvány lejár</span><span class="sxs-lookup"><span data-stu-id="d09f8-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="d09f8-103">A probléma megoldásához hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="d09f8-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="d09f8-104">Telepítse a Microsoft Azure Active Directory module for Windows PowerShell a számítógépre (ha a modul még nincs telepítve).</span><span class="sxs-lookup"><span data-stu-id="d09f8-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="d09f8-105">Ehhez nyissa meg az [Azure Active Directory PowerShell for Graph-ot.](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="d09f8-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="d09f8-106">Kövesse az AD FS "Az AD FS-jogkivonat-aláíró tanúsítvány lejárta" című szakaszának ["Hiba történt a webhely elérése közben" című hiba "Hiba történt a webhely elérése közben" című hiba lépéseit, amikor egy összevont felhasználó bejelentkezik az Office 365-be, az Azure-ba vagy az Intune-ba.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="d09f8-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="d09f8-107">Kövesse a[t. T. Összevont tartomány beállításainak frissítése vagy javítása az Office 365-ben, az Azure-ban vagy az Intune-ban](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)című t.</span><span class="sxs-lookup"><span data-stu-id="d09f8-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="d09f8-108">Az összevonási tanúsítványok megújításáról az [O365 és az Azure AD tanúsítványmegújítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="d09f8-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

