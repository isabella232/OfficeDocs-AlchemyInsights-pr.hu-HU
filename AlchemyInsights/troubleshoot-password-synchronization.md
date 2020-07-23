---
title: Jelszó-szinkronizálás – problémamegoldás
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387879"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f692f-102">Jelszó-szinkronizálás – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="f692f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f692f-103">A jelszó-szinkronizálási problémák elhárításához először használja ezt az AAD Connect hibaelhárítási feladatot annak megállapítására, hogy miért nem szinkronizálják a jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="f692f-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="f692f-104">A kezdéshez nyissa meg [a Közvetlen szinkronizálás kezelése](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)című.</span><span class="sxs-lookup"><span data-stu-id="f692f-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="f692f-105">Nyisson meg egy új Windows PowerShell-munkamenetet az Azure AD Connect-kiszolgálón, és válassza a **Futtatás rendszergazdaként** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f692f-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="f692f-106">Futtassa a Set-ExecutionPolicy RemoteSigned vagy Set-ExecutionPolicy Unrestricted (Set-ExecutionPolicy) futtatása korlátozás nélkül.</span><span class="sxs-lookup"><span data-stu-id="f692f-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="f692f-107">Indítsa el az Azure AD Connect varázslót.</span><span class="sxs-lookup"><span data-stu-id="f692f-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="f692f-108">Nyissa meg a További feladatok lapot > **Következő hibaelhárítást.**  >  **Next**</span><span class="sxs-lookup"><span data-stu-id="f692f-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="f692f-109">Válassza az **Indítás** lehetőséget a PowerShell hibaelhárítási menüjének megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="f692f-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="f692f-110">Válassza a **Jelszó-szinkronizálás hibaelhárítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="f692f-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="f692f-111">A probléma általában az, hogy a jelszó nincs szinkronizálva egy adott felhasználói fiókhoz.</span><span class="sxs-lookup"><span data-stu-id="f692f-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="f692f-112">**Megjegyzések** A jelszószinkronizálás sikertelen, ha az utolsó sikeres jelszószinkronizálás néhány évvel ezelőtt volt.</span><span class="sxs-lookup"><span data-stu-id="f692f-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="f692f-113">A jelszó-szinkronizálás hibaelhárításával kapcsolatos további segítségért olvassa el [A jelszókivonat-szinkronizálás hibaelhárítása az Azure AD Connect szinkronizálásával című témakört.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="f692f-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>