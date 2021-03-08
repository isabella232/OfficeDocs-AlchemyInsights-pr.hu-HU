---
title: A ClientAccessServerEnabled beállítása igazra
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524555"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="941d9-102">A ClientAccessServerEnabled beállítása igazra</span><span class="sxs-lookup"><span data-stu-id="941d9-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="941d9-103">Ha nem tud megnyitni egy titkosított e-mailt, és helyette egy **rpmsg** mellékletet lát, végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="941d9-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="941d9-104">Csatlakozás az Exchange Online PowerShellhez.</span><span class="sxs-lookup"><span data-stu-id="941d9-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="941d9-105">Az Exchange Online PowerShellhez való csatlakozáshoz globális rendszergazdai vagy Exchange-rendszergazdai fiókkal kell bejelentkeznie.</span><span class="sxs-lookup"><span data-stu-id="941d9-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="941d9-106">a.</span><span class="sxs-lookup"><span data-stu-id="941d9-106">a.</span></span> <span data-ttu-id="941d9-107">Nyissa meg a Windows PowerShellt, és futtassa a következő parancsot: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="941d9-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="941d9-108">b.</span><span class="sxs-lookup"><span data-stu-id="941d9-108">b.</span></span> <span data-ttu-id="941d9-109">A **Windows PowerShell hitelesítő** adatok kérése párbeszédpanelén adja meg munkahelyi vagy iskolai fiókját és jelszavát( c).</span><span class="sxs-lookup"><span data-stu-id="941d9-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="941d9-110">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="941d9-110">Click **OK**.</span></span> 

2. <span data-ttu-id="941d9-111">Új munkamenet létrehozásához futtassa az alábbi parancsot:</span><span class="sxs-lookup"><span data-stu-id="941d9-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="941d9-112">a.</span><span class="sxs-lookup"><span data-stu-id="941d9-112">a.</span></span> <span data-ttu-id="941d9-113">Futtassa a következő parancsot:</span><span class="sxs-lookup"><span data-stu-id="941d9-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="941d9-114">Futtatás `Get-IRMConfiguration` parancs.</span><span class="sxs-lookup"><span data-stu-id="941d9-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="941d9-115">Ellenőrizze **a ClientAccessServerEnabled beállítást.**</span><span class="sxs-lookup"><span data-stu-id="941d9-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="941d9-116">a.</span><span class="sxs-lookup"><span data-stu-id="941d9-116">a.</span></span> <span data-ttu-id="941d9-117">Ha **a ClientAccessServerEnabled** beállítása **Hamis,** futtassa az alábbi parancsmagot: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="941d9-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="941d9-118">Mindig zárja be a PowerShell-munkamenetet az alábbi paranccsal: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="941d9-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="941d9-119">További információ: [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="941d9-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

