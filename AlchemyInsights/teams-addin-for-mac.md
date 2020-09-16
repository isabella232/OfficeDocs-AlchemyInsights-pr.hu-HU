---
title: Mac Teams-bővítmény
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670330"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="3bcb3-102">Mac Teams-bővítmény</span><span class="sxs-lookup"><span data-stu-id="3bcb3-102">Teams add-in for Mac</span></span>

<span data-ttu-id="3bcb3-103">Ha meg szeretné tudni, hogy miként oldhatja meg a hiányzó Teams-bővítményt a Mac operációs rendszer felhasználóinak, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="3bcb3-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="3bcb3-104">**Lépés 1:** Ha a helyszíni hibrid Exchange (2016 CU3 vagy újabb verzió szükséges), az Test-HMA.ps1 eszközzel erősítse meg, hogy a hibrid, modern hitelesítés megfelelően van konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="3bcb3-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="3bcb3-105">További információt az [iOS és az Android rendszerhez készült hibrid, modern hitelesítés beállítása](https://aka.ms/AA980zq)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="3bcb3-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="3bcb3-106">**Note (Megjegyzés** ) Használja az UPN-címet (például [username@contoso.com](mailto:username@contoso.com)), ne TARTOMANY\felhasznalonev.</span><span class="sxs-lookup"><span data-stu-id="3bcb3-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="3bcb3-107">Ezt még a felhasználók számára is megteheti az Exchange Online-postaládákkal.</span><span class="sxs-lookup"><span data-stu-id="3bcb3-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="3bcb3-108">Második **lépés:** Használja a felhasználó a **Tools**-  >  **fiókok**lehetőséget. a Mac Outlookban, és keresse meg és jelölje ki a fiókot.</span><span class="sxs-lookup"><span data-stu-id="3bcb3-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="3bcb3-109">Ellenőrizze, hogy a megadott Felhasználónév UPN formátumú-e (például [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="3bcb3-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="3bcb3-110">**3. lépés:** Erősítse meg, hogy a felhasználó licencelt Microsoft Teams-felhasználó.</span><span class="sxs-lookup"><span data-stu-id="3bcb3-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="3bcb3-111">A felhasználónak a Mac Office 365-előfizetés, a Product 16,24-es vagy újabb verzióját kell használnia.</span><span class="sxs-lookup"><span data-stu-id="3bcb3-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>