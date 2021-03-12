---
title: Set ClientAccessServerEnabled to True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746414"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="a017e-102">Set ClientAccessServerEnabled to True</span><span class="sxs-lookup"><span data-stu-id="a017e-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="a017e-103">Ha nem tud megnyitni egy titkosított e-mailt, és helyette **egy rpmsg** mellékletet lát, végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="a017e-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="a017e-104">Csatlakozás az Exchange Online PowerShellhez.</span><span class="sxs-lookup"><span data-stu-id="a017e-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="a017e-105">Az Exchange Online PowerShellhez való csatlakozáshoz globális rendszergazdai vagy Exchange-rendszergazdai fiókkal kell bejelentkeznie.</span><span class="sxs-lookup"><span data-stu-id="a017e-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="a017e-106">a.</span><span class="sxs-lookup"><span data-stu-id="a017e-106">a.</span></span> <span data-ttu-id="a017e-107">Nyissa meg a Windows PowerShellt, és futtassa a következő parancsot: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="a017e-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="a017e-108">b.</span><span class="sxs-lookup"><span data-stu-id="a017e-108">b.</span></span> <span data-ttu-id="a017e-109">A **Windows PowerShell** hitelesítő adatok kérése párbeszédpanelen adja meg munkahelyi vagy iskolai fiókját és jelszavát, c.</span><span class="sxs-lookup"><span data-stu-id="a017e-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="a017e-110">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="a017e-110">Click **OK**.</span></span> 

2. <span data-ttu-id="a017e-111">Futtassa az alábbi parancsot új munkamenet létrehozásához:</span><span class="sxs-lookup"><span data-stu-id="a017e-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="a017e-112">a.</span><span class="sxs-lookup"><span data-stu-id="a017e-112">a.</span></span> <span data-ttu-id="a017e-113">Futtassa a következő parancsot:</span><span class="sxs-lookup"><span data-stu-id="a017e-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="a017e-114">Futtatás `Get-IRMConfiguration` parancs.</span><span class="sxs-lookup"><span data-stu-id="a017e-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="a017e-115">Ellenőrizze **a ClientAccessServerEnabled beállítást.**</span><span class="sxs-lookup"><span data-stu-id="a017e-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="a017e-116">a.</span><span class="sxs-lookup"><span data-stu-id="a017e-116">a.</span></span> <span data-ttu-id="a017e-117">Ha **a ClientAccessServerEnabled** beállítás **False (Hamis)** értéket ad meg, futtassa az alábbi parancsmagot: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="a017e-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="a017e-118">Mindig zárja be a PowerShell-munkamenetet a következő paranccsal: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="a017e-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="a017e-119">További információ: [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="a017e-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

