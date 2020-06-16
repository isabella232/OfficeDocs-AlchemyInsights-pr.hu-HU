---
title: A tulajdonos nem tud almappát létrehozni az Outlook programmal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748909"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="41b97-102">A tulajdonos nem tud almappát létrehozni az Outlook programmal</span><span class="sxs-lookup"><span data-stu-id="41b97-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="41b97-103">**Folyamatos probléma van azzal, hogy a nyilvános mappák tulajdonosai almappákat hoznak létre az Outlook programmal. A probléma hamarosan megoldódik.**</span><span class="sxs-lookup"><span data-stu-id="41b97-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="41b97-104">Eközben használja az alábbi megoldások egyikét:</span><span class="sxs-lookup"><span data-stu-id="41b97-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="41b97-105">Az almappa létrehozása a MAC Outlook programmal, mivel a probléma csak az asztali Outlook ablakait érinti (az összes verzió)</span><span class="sxs-lookup"><span data-stu-id="41b97-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="41b97-106">Az almappa létrehozása az EXO Rendszerhéj vagy az EAC használatával</span><span class="sxs-lookup"><span data-stu-id="41b97-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="41b97-107">A felhasználó alapértelmezettPublicFoldermailbox/effectivePublicfoldermailbox fájljának módosítása más postaládára, mint a problémát okozó mappa Tartalompostaládája</span><span class="sxs-lookup"><span data-stu-id="41b97-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="41b97-108">*Set-mailbox User1 alapértelmezettPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="41b97-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="41b97-109">Várjon egy órát, indítsa újra az Outlook-ügyfelet</span><span class="sxs-lookup"><span data-stu-id="41b97-109">Wait for an hour, restart outlook client</span></span>