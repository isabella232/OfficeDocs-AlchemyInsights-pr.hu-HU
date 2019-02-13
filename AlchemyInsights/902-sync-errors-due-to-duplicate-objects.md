---
title: 902 (szinkronizálási hibák miatt az ismétlődő objektumok)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919874"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="dfabc-102">A szinkronizálási hibák miatt az ismétlődő objektumok</span><span class="sxs-lookup"><span data-stu-id="dfabc-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="dfabc-103">Az alábbi hibaüzenetek egyike jelenhet directory szinkronizálásának befejeztével:</span><span class="sxs-lookup"><span data-stu-id="dfabc-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="dfabc-104">Nem lehet frissíteni az objektumot a Microsoft Online Services, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi könyvtárban egy másik objektumhoz társított.</span><span class="sxs-lookup"><span data-stu-id="dfabc-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="dfabc-105">A szinkronizált objektumok proxy címe megegyezik a Microsoft Online Services könyvtárban már létezik.</span><span class="sxs-lookup"><span data-stu-id="dfabc-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="dfabc-106">Nem lehet frissíteni az objektum, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi címtárszolgáltatás a másik objektumhoz társított: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="dfabc-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="dfabc-107">Azonosítására, és a probléma megoldásához töltse le és futtassa a [IdFix DirSync hiba javítására szolgáló eszköz](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="dfabc-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="dfabc-108">További tudnivalókért lásd: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="dfabc-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

