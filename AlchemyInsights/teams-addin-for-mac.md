---
title: Teams Mac bővítmény
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582072"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="6bc34-102">Teams Mac bővítmény</span><span class="sxs-lookup"><span data-stu-id="6bc34-102">Teams add-in for Mac</span></span>

<span data-ttu-id="6bc34-103">Ha el szeretne hárítani egy hiányzó Teams maces operációsrendszer-felhasználóknak, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="6bc34-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="6bc34-104">**1. lépés:** Ha hibrid hibrid Exchange (2016 CU3 vagy újabb szükséges), az Test-HMA.ps1 eszközzel győződjön meg arról, hogy a hibrid modern hitelesítés megfelelően van konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="6bc34-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="6bc34-105">További információ: A hibrid modern hitelesítés beállítása [iOS](https://aka.ms/TestHMAEAS)és Android Outlook esetén.</span><span class="sxs-lookup"><span data-stu-id="6bc34-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="6bc34-106">**Megjegyzés** Használja az UPN-címformátumot [(például username@contoso.com](mailto:username@contoso.com)), és ne a tartomán\felhasználónév formátumot.</span><span class="sxs-lookup"><span data-stu-id="6bc34-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="6bc34-107">Még a postaládával is Exchange Online felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="6bc34-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="6bc34-108">**2. lépés:** A felhasználónak az Eszközök **fiókok...**  >   lehetőséget Mac Outlook, majd keresse meg és jelölje ki a fiókot.</span><span class="sxs-lookup"><span data-stu-id="6bc34-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="6bc34-109">Győződjön meg arról, hogy a felsorolt felhasználónév UPN formátumban van (például [username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="6bc34-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="6bc34-110">**3. lépés:** Győződjön meg arról, hogy a felhasználó licencelt Microsoft Teams felhasználó.</span><span class="sxs-lookup"><span data-stu-id="6bc34-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="6bc34-111">A felhasználónak a Mac Office 365 16.24-es vagy újabb termékverzióját kell használnia.</span><span class="sxs-lookup"><span data-stu-id="6bc34-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>