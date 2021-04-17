---
title: Nem lehet hozzáférni a nyilvános mappákhoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819514"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="670a8-102">Az Outlook nem tud nyilvános mappákhoz csatlakozni</span><span class="sxs-lookup"><span data-stu-id="670a8-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="670a8-103">Ha egyes felhasználók számára nem működik a nyilvános mappa elérése, próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="670a8-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="670a8-104">Csatlakozzon az EXO PowerShellhez, és állítsa be a DefaultPublicFolderMailbox paramétert a problémás felhasználói fiókon úgy, hogy megfeleljen egy működő felhasználói fiók paraméterének.</span><span class="sxs-lookup"><span data-stu-id="670a8-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="670a8-105">Példa:</span><span class="sxs-lookup"><span data-stu-id="670a8-105">Example:</span></span>

<span data-ttu-id="670a8-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="670a8-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="670a8-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="670a8-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="670a8-108">Várjon legalább egy órát, amíg a módosítás életbe lép.</span><span class="sxs-lookup"><span data-stu-id="670a8-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="670a8-109">Ha a probléma továbbra [](https://aka.ms/pfcte) is fennáll, kövesse az alábbi eljárást a nyilvános mappák elérésével kapcsolatos problémák elhárításához az Outlookkal.</span><span class="sxs-lookup"><span data-stu-id="670a8-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="670a8-110">**Annak szabályozása, hogy mely felhasználók férnek hozzá a nyilvános mappákhoz az Outlook használatával:**</span><span class="sxs-lookup"><span data-stu-id="670a8-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="670a8-111">Használja Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true vagy $false</span><span class="sxs-lookup"><span data-stu-id="670a8-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="670a8-112">$true: Nyilvános mappák elérésének engedélyezése a felhasználóknak az Outlookban</span><span class="sxs-lookup"><span data-stu-id="670a8-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="670a8-113">$false: Felhasználói hozzáférés megakadályozása a nyilvános mappákhoz az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="670a8-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="670a8-114">Ez az alapértelmezett érték.</span><span class="sxs-lookup"><span data-stu-id="670a8-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="670a8-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="670a8-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="670a8-116">**Megjegyzés** Ez az eljárás csak a Windows Outlook asztali verziójával létesítő kapcsolatokat szabályozhatja.</span><span class="sxs-lookup"><span data-stu-id="670a8-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="670a8-117">A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az OWA vagy a Mac Outlook használatával.</span><span class="sxs-lookup"><span data-stu-id="670a8-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="670a8-118">További információ: [Az Outlookban](https://aka.ms/controlpf)a nyilvános mappákhoz való szabályozott kapcsolatok támogatása.</span><span class="sxs-lookup"><span data-stu-id="670a8-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>