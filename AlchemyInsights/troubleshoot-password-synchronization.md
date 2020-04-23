---
title: Jelszó-szinkronizálás – problémamegoldás
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
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732512"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="feac3-102">Jelszó-szinkronizálás – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="feac3-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="feac3-103">Olyan problémák elhárítása, amelyek miatt nincsenek jelszavak szinkronizálása az Azure AD Connect 1.1.614.0-s vagy újabb verziójával:</span><span class="sxs-lookup"><span data-stu-id="feac3-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="feac3-104">Nyisson meg egy új Windows PowerShell-munkamenetet az Azure AD Connect kiszolgálón a **Futtatás rendszergazdaként** beállítással.</span><span class="sxs-lookup"><span data-stu-id="feac3-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="feac3-105">Futtassa **a Set-ExecutionPolicy RemoteSigned** vagy **Set-ExecutionPolicy Unrestricted (Set-ExecutionPolicy ) futtatása korlátozás nélkül.**</span><span class="sxs-lookup"><span data-stu-id="feac3-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="feac3-106">Indítsa el az Azure AD Connect varázslót.</span><span class="sxs-lookup"><span data-stu-id="feac3-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="feac3-107">Nyissa meg a **További feladatok** lapot, válassza **a Hibaelhárítás**lehetőséget, és kattintson a **Tovább**gombra.</span><span class="sxs-lookup"><span data-stu-id="feac3-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="feac3-108">A Hibaelhárítás lapon kattintson az Indítás gombra a PowerShell hibaelhárítási menüjének **elindításához.**</span><span class="sxs-lookup"><span data-stu-id="feac3-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="feac3-109">A főmenüben válassza a **Jelszó-szinkronizálás hibaelhárítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="feac3-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="feac3-110">Az almenüben válassza a **Jelszó-szinkronizálás parancs átnem nem működik.**</span><span class="sxs-lookup"><span data-stu-id="feac3-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="feac3-111">**A hibaelhárítási feladat eredményeinek megismerése**</span><span class="sxs-lookup"><span data-stu-id="feac3-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="feac3-112">A hibaelhárítási feladat a következő ellenőrzéseket hajtja végre:</span><span class="sxs-lookup"><span data-stu-id="feac3-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="feac3-113">Ellenőrzi, hogy a jelszó-szinkronizálási funkció engedélyezve van-e az Azure AD-bérlőhöz.</span><span class="sxs-lookup"><span data-stu-id="feac3-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="feac3-114">Ellenőrzi, hogy az Azure AD Connect-kiszolgáló nincs-e átmeneti módban.</span><span class="sxs-lookup"><span data-stu-id="feac3-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="feac3-115">Minden meglévő helyszíni Active Directory-összekötő esetén (amely egy meglévő Active Directory-erdőnek felel meg):</span><span class="sxs-lookup"><span data-stu-id="feac3-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="feac3-116">Ellenőrzi, hogy a jelszó-szinkronizálási szolgáltatás engedélyezve van-e.</span><span class="sxs-lookup"><span data-stu-id="feac3-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="feac3-117">Jelszó-szinkronizálási szívverési események keresése a Windows alkalmazás eseménynaplóiban.</span><span class="sxs-lookup"><span data-stu-id="feac3-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="feac3-118">A helyszíni Active Directory-összekötő alatti minden Egyes Active Directory-tartomány esetén:</span><span class="sxs-lookup"><span data-stu-id="feac3-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="feac3-119">Ellenőrzi, hogy a tartomány elérhető-e az Azure AD Connect-kiszolgálóról.</span><span class="sxs-lookup"><span data-stu-id="feac3-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="feac3-120">Ellenőrzi, hogy a helyszíni Active Directory-összekötő által használt Active Directory tartományi szolgáltatások (AD DS) fiókok rendelkeznek-e a jelszó-szinkronizáláshoz szükséges megfelelő felhasználónévvel, jelszóval és engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="feac3-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="feac3-121">A jelszószinkronizálás hibaelhárításával kapcsolatos további segítségért olvassa el a [Jelszó-szinkronizálás hibaelhárítása az Azure AD Connect szinkronizálásával című témakört.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)</span><span class="sxs-lookup"><span data-stu-id="feac3-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  