---
title: A tulajdonos nem tud almappát létrehozni az Outlookkal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665720"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="ccd99-102">A tulajdonos nem tud almappát létrehozni az Outlookkal</span><span class="sxs-lookup"><span data-stu-id="ccd99-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="ccd99-103">**Folyamatban van egy probléma a nyilvános mappák tulajdonosainak az Outlookkal való létrehozásakor. A probléma hamarosan kijavításra kerül.**</span><span class="sxs-lookup"><span data-stu-id="ccd99-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="ccd99-104">Eközben használja az alábbi kerülő megoldások egyikét:</span><span class="sxs-lookup"><span data-stu-id="ccd99-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="ccd99-105">A MAC Outlook használata az almappa létrehozásához a probléma hatása csak az asztali Windows Outlook (minden verzió)</span><span class="sxs-lookup"><span data-stu-id="ccd99-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="ccd99-106">A rendszergazda hozza létre az almappát az EXO Shell vagy az EAC segítségével</span><span class="sxs-lookup"><span data-stu-id="ccd99-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="ccd99-107">A felhasználó DefaultPublicFolderMailbox/EffectivePublicFolderMailbox módosítása a problémát okozó mappa tartalmát tartalmazó postaládára</span><span class="sxs-lookup"><span data-stu-id="ccd99-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="ccd99-108">*Set-Mailbox Felhasználó1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="ccd99-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="ccd99-109">Várjon egy órát, indítsa újra az Outlook ügyfélprogramot</span><span class="sxs-lookup"><span data-stu-id="ccd99-109">Wait for an hour, restart outlook client</span></span>