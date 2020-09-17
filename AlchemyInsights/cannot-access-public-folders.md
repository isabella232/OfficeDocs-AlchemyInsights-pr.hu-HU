---
title: Nem érhetők el a nyilvános mappák
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812549"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="95908-102">Az Outlook nem tud csatlakozni nyilvános mappákhoz</span><span class="sxs-lookup"><span data-stu-id="95908-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="95908-103">Ha a nyilvános mappákhoz való hozzáférés néhány felhasználónál nem működött, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="95908-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="95908-104">Csatlakozzon az EXO PowerShellhez, és állítsa be a DefaultPublicFolderMailbox paramétert a problémás felhasználói fiókban, hogy megegyezzenek a megfelelő felhasználói fiók paraméterével.</span><span class="sxs-lookup"><span data-stu-id="95908-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="95908-105">Például</span><span class="sxs-lookup"><span data-stu-id="95908-105">Example:</span></span>

<span data-ttu-id="95908-106">Get-Mailbox WorkingUser | Ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="95908-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="95908-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="95908-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="95908-108">Várjon legalább egy órát, amíg a módosítás érvénybe lép.</span><span class="sxs-lookup"><span data-stu-id="95908-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="95908-109">Ha a probléma továbbra is fennáll, kérjük, kövesse az alábbi [lépéseket](https://aka.ms/pfcte) a nyilvános mappák elérésével kapcsolatos hibák elhárítása az Outlookkal.</span><span class="sxs-lookup"><span data-stu-id="95908-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="95908-110">**Annak szabályozása, hogy mely felhasználók érhetik el nyilvános mappákat az Outlookkal**:</span><span class="sxs-lookup"><span data-stu-id="95908-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="95908-111">Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE vagy $FALSE</span><span class="sxs-lookup"><span data-stu-id="95908-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="95908-112">$true: hozzáférés engedélyezése a felhasználóknak nyilvános mappákhoz az Outlookban</span><span class="sxs-lookup"><span data-stu-id="95908-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="95908-113">$false: felhasználók hozzáférésének megakadályozása az Outlookban elérhető nyilvános mappákhoz.</span><span class="sxs-lookup"><span data-stu-id="95908-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="95908-114">Ez az alapértelmezett érték.</span><span class="sxs-lookup"><span data-stu-id="95908-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="95908-115">Set-OrganizationalSetting-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="95908-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="95908-116">**Note (Megjegyzés** ) Ez az eljárás csak a Windows Outlook asztali verziókkal használható a kapcsolat vezérlésére.</span><span class="sxs-lookup"><span data-stu-id="95908-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="95908-117">A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az OWA vagy a Mac Outlook használatával.</span><span class="sxs-lookup"><span data-stu-id="95908-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="95908-118">További információt az [ellenőrzött kapcsolatok támogatása a nyilvános mappákhoz az Outlookban](https://aka.ms/controlpf)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="95908-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>