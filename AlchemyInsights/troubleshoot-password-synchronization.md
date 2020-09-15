---
title: Jelszó-szinkronizálás hibaelhárítása
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
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664928"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="b4337-102">Jelszó-szinkronizálás hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="b4337-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="b4337-103">A jelszó-szinkronizálási hibák elhárításához Kezdje a AAD csatlakoztatása hibaelhárítási feladattal annak megállapításához, hogy miért nem szinkronizálja a jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="b4337-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="b4337-104">A kezdéshez lépjen a [közvetlen szinkronizálás kezelése](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)elemre.</span><span class="sxs-lookup"><span data-stu-id="b4337-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="b4337-105">Nyisson meg egy új Windows PowerShell-munkamenetet az Azure AD Connect-kiszolgálón, és válassza a **Futtatás rendszergazdaként** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b4337-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="b4337-106">Futtassa a Set-ExecutionPolicy RemoteSigned vagy a Set-ExecutionPolicy korlátozás nélküli beállítást.</span><span class="sxs-lookup"><span data-stu-id="b4337-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="b4337-107">Indítsa el az Azure AD Connect varázslót.</span><span class="sxs-lookup"><span data-stu-id="b4337-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="b4337-108">Lépjen a további feladatok lapra > **Hibaelhárítás**című témakört  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="b4337-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="b4337-109">Válassza az **Indítás** gombot a PowerShell hibaelhárítási menüjének megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="b4337-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="b4337-110">Válassza a **Jelszó-szinkronizálás elhárítása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b4337-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="b4337-111">A probléma általában az, hogy egy adott felhasználói fiókhoz nincs szinkronizálva jelszó.</span><span class="sxs-lookup"><span data-stu-id="b4337-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="b4337-112">**Megjegyzések** A jelszó-szinkronizálás sikertelen, ha az utolsó sikeres jelszó-szinkronizálás néhány évvel ezelőtt volt.</span><span class="sxs-lookup"><span data-stu-id="b4337-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="b4337-113">A jelszó-szinkronizálással kapcsolatos további segítségért olvassa el a [jelszó-ujjlenyomat szinkronizálása az Azure ad Connect szinkronizálásával](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)című témakört.</span><span class="sxs-lookup"><span data-stu-id="b4337-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>