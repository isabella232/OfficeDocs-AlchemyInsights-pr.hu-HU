---
title: 902 (Szinkronizálási hibák ismétlődő objektumok miatt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767130"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="95698-102">Ismétlődő objektumok miatti szinkronizálási hibák</span><span class="sxs-lookup"><span data-stu-id="95698-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="95698-103">A Microsoft 365-ben a címtár-szinkronizálás befejezésekor az alábbi hibaüzenetek egyike jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="95698-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="95698-104">Az objektum nem frissíthető a Microsoft Online Services szolgáltatásban, mert az objektumhoz társított alábbi attribútumok olyan értékekkel rendelkeznek, amelyek már társítva lehetnek a helyi címtár egy másik objektumával.</span><span class="sxs-lookup"><span data-stu-id="95698-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="95698-105">Már létezik ugyanazzal a proxycímmel rendelkező szinkronizált objektum a Microsoft Online Services címtárban.</span><span class="sxs-lookup"><span data-stu-id="95698-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="95698-106">Az objektum nem frissíthető, mert az objektumhoz társított következő attribútumok olyan értékekkel rendelkeznek, amelyek már társítva lehetnek a helyi címtárszolgáltatások egy másik objektumával: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="95698-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="95698-107">A probléma azonosításához és javításához töltse le és futtassa az [IdFix DirSync hibajavító eszközt.](https://www.microsoft.com/download/details.aspx?id=36832)</span><span class="sxs-lookup"><span data-stu-id="95698-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="95698-108">További információ: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="95698-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
