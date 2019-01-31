---
title: ADFS összevonási tanúsítvány ennyi időn belül lejár
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 6170265dac1eebe8fa1acf766d2eb8d6b0a5908b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662365"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="10c08-102">ADFS összevonási tanúsítvány ennyi időn belül lejár</span><span class="sxs-lookup"><span data-stu-id="10c08-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="10c08-103">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="10c08-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="10c08-p101">A Microsoft Azure Active Directory modult a Windows PowerShell telepítése a számítógépen (Ha a modul nincs még telepítve). Ehhez lépjen [kezelése a Windows PowerShell Azure AD](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="10c08-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="10c08-106">Kövesse az "1. eset: az AD FS-jogkivonat-aláíró tanúsítvány lejárt" részében a ["Hiba történt a webhely eléréséhez" hiba az Active Directory összevonási szolgáltatások összevont felhasználó bejelentkezik az Office 365, Azure, vagy Intune esetén](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="10c08-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="10c08-107">Kövesse a [frissítés, vagy a beállításokat az Office 365, Azure, vagy Intune összevont tartomány javítása](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="10c08-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="10c08-108">További információ összevonási ismerhet [Office 365 és Azure az Active Directory összevonási tanúsítványok megújítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="10c08-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

