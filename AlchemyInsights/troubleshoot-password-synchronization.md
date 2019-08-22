---
title: A jelszó-szinkronizálás hibaelhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533809"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="3d700-102">A jelszó-szinkronizálás hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="3d700-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="3d700-103">Nincs jelszó esetén szinkronizált Azure AD csatlakozás verziója 1.1.614.0 vagy annál újabb problémák elhárításához:</span><span class="sxs-lookup"><span data-stu-id="3d700-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="3d700-104">Nyissa meg a Azure AD csatlakozás kiszolgálón egy új Windows PowerShell munkamenetet a **Futtatás rendszergazdaként** beállítással.</span><span class="sxs-lookup"><span data-stu-id="3d700-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="3d700-105">Futtassa a **Set-ExecutionPolicy RemoteSigned** vagy a **Set-ExecutionPolicy korlátlan**.</span><span class="sxs-lookup"><span data-stu-id="3d700-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="3d700-106">Borzas AD csatlakozás varázsló elindításához.</span><span class="sxs-lookup"><span data-stu-id="3d700-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="3d700-107">A **További feladatok** lapra, jelölje ki a **Hibaelhárítás**, és kattintson a **Tovább**gombra.</span><span class="sxs-lookup"><span data-stu-id="3d700-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="3d700-108">A hibaelhárítás lapon kattintson **a hibaelhárítás mikéntje az indítási** menü a PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3d700-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="3d700-109">Válassza a főmenü, **A jelszó-szinkronizálás hibaelhárítása**.</span><span class="sxs-lookup"><span data-stu-id="3d700-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="3d700-110">Válassza ki a sub menü **Jelszó-szinkronizálás egyáltalán nem működik**.</span><span class="sxs-lookup"><span data-stu-id="3d700-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="3d700-111">**A hibaelhárítási feladat az eredmények értelmezésében**</span><span class="sxs-lookup"><span data-stu-id="3d700-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="3d700-112">A hibaelhárítási feladat a következő ellenőrzéseket hajtja végre:</span><span class="sxs-lookup"><span data-stu-id="3d700-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="3d700-113">Ellenőrzi, hogy a jelszó-szinkronizálás szolgáltatás engedélyezve van a Azure AD bérlő.</span><span class="sxs-lookup"><span data-stu-id="3d700-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="3d700-114">Ellenőrzi, hogy a Borzas AD csatlakozás kiszolgáló nincs a fejlesztői üzemmód.</span><span class="sxs-lookup"><span data-stu-id="3d700-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="3d700-115">Minden meglévő helyszíni Active Directory Connector (amely megfelel a meglévő Active Directory-erdő):</span><span class="sxs-lookup"><span data-stu-id="3d700-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="3d700-116">Ellenőrzi, hogy a jelszó-szinkronizálás szolgáltatás engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="3d700-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="3d700-117">Jelszó szinkronizálás szívverés események a Windows alkalmazás-eseménynaplókban keres.</span><span class="sxs-lookup"><span data-stu-id="3d700-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="3d700-118">Minden egyes Active Directory tartomány alapján a helyszíni Active Directory-csatoló:</span><span class="sxs-lookup"><span data-stu-id="3d700-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="3d700-119">Ellenőrzi, hogy a tartomány a Azure AD csatlakozás kiszolgálóról érhető.</span><span class="sxs-lookup"><span data-stu-id="3d700-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="3d700-120">Ellenőrzi, hogy a helyszíni Active Directory-csatolója az Active Directory tartományi szolgáltatások (AD DS) fiókokat rendelkezik-e a helyes felhasználónév, jelszó és a jelszó-szinkronizálás szükséges engedélyek.</span><span class="sxs-lookup"><span data-stu-id="3d700-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="3d700-121">Jelszó-szinkronizálás hibáinak elhárítása További segítséget talál [Azure AD csatlakozás szinkronizálás a jelszó-szinkronizálás hibaelhárítása](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="3d700-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  