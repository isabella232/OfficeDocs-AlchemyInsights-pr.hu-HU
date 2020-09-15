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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="4d737-102">Az ADFS-összevonási tanúsítvány lejárata</span><span class="sxs-lookup"><span data-stu-id="4d737-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="4d737-103">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="4d737-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="4d737-104">Telepítse a Windows PowerShellhez készült Microsoft Azure Active Directory modult a számítógépen (ha még nincs telepítve a modul).</span><span class="sxs-lookup"><span data-stu-id="4d737-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="4d737-105">Ehhez nyissa meg az [Azure ad kezelése a Windows PowerShell használatával](https://aka.ms/aadposh)című cikk lépéseit.</span><span class="sxs-lookup"><span data-stu-id="4d737-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="4d737-106">Kövesse a következő témakörben szereplő lépéseket: az AD FS-jogkivonat-aláíró tanúsítvány lejárt "az [" nem sikerült elérni a webhelyet "hibaüzenet jelenik meg az AD FS-ből, ha egy szövetséges felhasználó bejelentkezik a Microsoft 365, Azure vagy Intune szolgáltatásba](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="4d737-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="4d737-107">Kövesse a következő témakör lépéseit: az [összevont tartományok frissítése vagy javítása a Microsoft, Azure vagy Intune környezetben](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="4d737-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="4d737-108">Ha többet szeretne tudni az összevonási tanúsítványok megújításáról, olvassa el [az összevonási tanúsítványok megújítása a Microsoft 365 és az Azure Active Directory szolgáltatásban](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakört.</span><span class="sxs-lookup"><span data-stu-id="4d737-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
