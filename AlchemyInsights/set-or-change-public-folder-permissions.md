---
title: Nyilvánosmappa-engedélyek beállítása vagy módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36734671"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="c12d7-102">Engedélyek és nyilvános mappák</span><span class="sxs-lookup"><span data-stu-id="c12d7-102">Permissions and Public Folders</span></span>

<span data-ttu-id="c12d7-103">Az Outlook, az Exchange Admin Center (EAC) vagy a PowerShell segítségével módosíthatja a nyilvános mappák engedélyeit:</span><span class="sxs-lookup"><span data-stu-id="c12d7-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="c12d7-104">Az Outlook utasításokért [kattintson ide](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="c12d7-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="c12d7-105">Az EAC-ra vonatkozó útmutatásokért olvassa el [ezt a cikket](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) .</span><span class="sxs-lookup"><span data-stu-id="c12d7-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="c12d7-106">Részére PowerShell, folyamodik [Ez cikk](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) részére oktatás-ra használ a összead-PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="c12d7-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="c12d7-107">Ha az Exchange PowerShell eszközzel való csatlakozáshoz útmutatásra van szüksége, kattintson [ide](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="c12d7-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="c12d7-108">Ha **külső felhasználók nem tudnak e-maileket küldeni egy levelezési nyilvános mappába**, ennek oka lehet, hogy a nyilvános mappa nem rendelkezik a külső e-mail kézbesítéshez szükséges engedélyekkel.</span><span class="sxs-lookup"><span data-stu-id="c12d7-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="c12d7-109">Ezt a javítást az Outlook utasításaival, [illetve a PowerShell útmutatásai](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)segítségével is kijavíthatja [.](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="c12d7-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

