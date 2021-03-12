---
title: 902 (Szinkronizálási hibák az ismétlődő objektumok miatt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708064"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="6fd85-102">Szinkronizálási hibák duplikált objektumok miatt</span><span class="sxs-lookup"><span data-stu-id="6fd85-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="6fd85-103">Ha a címtár-szinkronizálás befejeződött a Microsoft 365-ben, az alábbi hibaüzenetek egyike jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="6fd85-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="6fd85-104">Nem lehet frissíteni ezt az objektumot a Microsoft Online Services szolgáltatásban, mert az objektumhoz tartozó alábbi attribútumok olyan értékeket tartalmaznak, amelyek már a helyi címtár egy másik objektumához vannak társítva.</span><span class="sxs-lookup"><span data-stu-id="6fd85-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="6fd85-105">Már létezik szinkronizált objektum ugyanazokkal a proxycímekkel a Microsoft Online Services címtárában.</span><span class="sxs-lookup"><span data-stu-id="6fd85-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="6fd85-106">Nem lehet frissíteni ezt az objektumot, mert az objektumhoz tartozó alábbi attribútumok olyan értékeket tartalmaznak, amelyek a helyi címtárszolgáltatások egy másik objektumához vannak társítva: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="6fd85-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="6fd85-107">A probléma azonosításához és megoldásához töltse le és futtassa az [IdFix DirSync hibajavítási eszközt.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="6fd85-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="6fd85-108">További információ: [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="6fd85-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
