---
title: A tulajdonos nem hozhat létre almappát az Outlookkal
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836137"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="c6312-102">A tulajdonos nem hozhat létre almappát az Outlookkal</span><span class="sxs-lookup"><span data-stu-id="c6312-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="c6312-103">**Egy még folyamatban lévő hiba miatt a nyilvános mappatulajdonosok az Outlook segítségével hoznak létre almappákat. A problémát hamarosan kijavítjuk.**</span><span class="sxs-lookup"><span data-stu-id="c6312-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="c6312-104">Addig is használja az alábbi kerülő megoldásokat:</span><span class="sxs-lookup"><span data-stu-id="c6312-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="c6312-105">Az almappa létrehozása a MAC Outlookkal, mivel a probléma csak az asztali Outlookot (az összes verziót) érintette.</span><span class="sxs-lookup"><span data-stu-id="c6312-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="c6312-106">Az almappa exo shell vagy EAC használatával való létrehozása a rendszergazdával</span><span class="sxs-lookup"><span data-stu-id="c6312-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="c6312-107">A problémát okozó mappa DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-jának módosítása a tartalompostaládán kívül más postaládára</span><span class="sxs-lookup"><span data-stu-id="c6312-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="c6312-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="c6312-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="c6312-109">Várjon egy órát, indítsa újra az Outlook ügyfélprogramot</span><span class="sxs-lookup"><span data-stu-id="c6312-109">Wait for an hour, restart outlook client</span></span>