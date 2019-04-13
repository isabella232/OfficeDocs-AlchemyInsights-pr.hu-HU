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
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859106"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="f2ec0-102">A szinkronizálási hibák miatt az ismétlődő objektumok</span><span class="sxs-lookup"><span data-stu-id="f2ec0-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="f2ec0-103">Az alábbi hibaüzenetek egyike jelenhet directory szinkronizálásának befejeztével:</span><span class="sxs-lookup"><span data-stu-id="f2ec0-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="f2ec0-104">Nem lehet frissíteni az objektumot a Microsoft Online Services, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi könyvtárban egy másik objektumhoz társított.</span><span class="sxs-lookup"><span data-stu-id="f2ec0-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="f2ec0-105">A szinkronizált objektumok proxy címe megegyezik a Microsoft Online Services könyvtárban már létezik.</span><span class="sxs-lookup"><span data-stu-id="f2ec0-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="f2ec0-106">Nem lehet frissíteni az objektum, mert a következő attribútumok az objektumhoz társított értékeket, amelyek esetleg már a helyi címtárszolgáltatás a másik objektumhoz társított: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f2ec0-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="f2ec0-107">Azonosítására, és a probléma megoldásához töltse le és futtassa a [IdFix DirSync hiba javítására szolgáló eszköz](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="f2ec0-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="f2ec0-108">További tudnivalókért lásd: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="f2ec0-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
