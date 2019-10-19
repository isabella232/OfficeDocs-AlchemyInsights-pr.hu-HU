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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737191"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="c9a84-102">Az ADFS összevonási tanúsítványának lejárása</span><span class="sxs-lookup"><span data-stu-id="c9a84-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="c9a84-103">A probléma megoldásához hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="c9a84-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="c9a84-104">A Microsoft Azure Active Directory-modul telepítése a számítógépre a Windows PowerShell környezethez (ha a modul még nincs telepítve).</span><span class="sxs-lookup"><span data-stu-id="c9a84-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="c9a84-105">Ehhez nyissa meg a [Windows PowerShell eszközzel a Azure rendszer kezelését](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="c9a84-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="c9a84-106">Kövesse a "1. forgatókönyv: az Active Directory összevonási szolgáltatások jogkivonat-aláíró tanúsítványa lejárt" című szakaszt "a [hely elérésekor hiba történt" hibaüzenet, amikor egy szövetséges felhasználó bejelentkezik az Office 365, Azure vagy Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)szolgáltatásba,</span><span class="sxs-lookup"><span data-stu-id="c9a84-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="c9a84-107">Kövesse a frissítés lépéseit, [vagy javítsa az összevont tartomány beállításait az Office 365, Azure vagy Intune tartományban](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="c9a84-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="c9a84-108">További információt az összevonási tanúsítványok megújításáról [az Office 365 és a Azure Active Directory összevonási tanúsítványainak megújítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c9a84-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
