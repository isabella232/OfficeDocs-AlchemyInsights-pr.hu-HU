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
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="1747e-102">Az egyik helyszíni összevonási szolgáltatási tanúsítvány lejár</span><span class="sxs-lookup"><span data-stu-id="1747e-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="1747e-103">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="1747e-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="1747e-104">Telepítse a Windows PowerShellhez készült Microsoft Azure Active Directory modult a számítógépen (ha még nincs telepítve a modul).</span><span class="sxs-lookup"><span data-stu-id="1747e-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="1747e-105">Ehhez nyissa meg az [Azure Active Directory PowerShellt a Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) -hoz.</span><span class="sxs-lookup"><span data-stu-id="1747e-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="1747e-106">Kövesse a következő témakörben szereplő lépéseket: az AD FS-jogkivonat-aláíró tanúsítvány lejárt "az [" nem sikerült elérni a webhelyet "hibaüzenet jelenik meg az AD FS-ből, ha egy szövetséges felhasználó bejelentkezik a Microsoft 365, Azure vagy Intune szolgáltatásba](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="1747e-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="1747e-107">Kövesse a következő témakör lépéseit: a [Microsoft 365, Azure vagy Intune rendszerbeli összevont tartományok beállításainak frissítése vagy kijavítása](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="1747e-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="1747e-108">Az összevonási tanúsítványok megújításáról további információt a [tanúsítvány megújítása a O365 és az Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)szolgáltatáshoz című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="1747e-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

