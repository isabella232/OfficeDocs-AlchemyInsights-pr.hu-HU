---
title: 182 kérjük, hogy az Outlook hitelesítési hibáinak diagnosztizálása és megoldása érdekében futtassa az SaRA alkalmazást.
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: aa1e831eac829f3bd35f34e2fbe34923c5af0d3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47802023"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="41f52-102">Az Outlook hitelesítési problémáinak diagnosztizálása és megoldása a SaRA használatával</span><span class="sxs-lookup"><span data-stu-id="41f52-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="41f52-103">**Megjegyzés**: Kérjük, ellenőrizze, hogy engedélyezve van-e a [biztonsági alapértékek](https://aka.ms/securitydefaults) a szervezetében.</span><span class="sxs-lookup"><span data-stu-id="41f52-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="41f52-104">Ha bérlője október 21 után jött létre, az 2019 és az Outlook ismétlődően kéri a jelszó megadását, lehet, hogy a bérlőben engedélyezve van a **biztonsági alapbeállítás** .</span><span class="sxs-lookup"><span data-stu-id="41f52-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="41f52-105">Javasoljuk, hogy az [Outlook továbbra is kéri a jelszó](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) -diagnosztikai szolgáltatás használatát az érintett gépen, és hárítsa el azokat a hibákat, amelyekkel az Outlook folyamatosan kéri a jelszó megadását.</span><span class="sxs-lookup"><span data-stu-id="41f52-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="41f52-106">Ez a [SaRA](https://diagnostics.office.com/#/) -diagnosztika automatizált ellenőrzéseket hajt végre, és az észlelt problémák megoldására szolgál a lehetséges megoldásokkal.</span><span class="sxs-lookup"><span data-stu-id="41f52-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
