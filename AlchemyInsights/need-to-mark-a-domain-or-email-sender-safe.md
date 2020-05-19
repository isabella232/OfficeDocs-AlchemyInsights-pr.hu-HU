---
title: Meg kell jelölnie egy tartomány- vagy e-mail feladói széfet?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281150"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="8d01a-102">Meg kell jelölnie egy tartomány- vagy e-mail feladói széfet?</span><span class="sxs-lookup"><span data-stu-id="8d01a-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="8d01a-103">A **biztonságos feladói listák** használata nem ajánlott, mivel megnyitja a szervezetet a levélszemét, a phish és a hamisítás igéző támadásai számára.</span><span class="sxs-lookup"><span data-stu-id="8d01a-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="8d01a-104">Ha azonban üzleti követelmény van, **javasoljuk, hogy** ehhez használja a **[Mail Flow-szabályokat.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="8d01a-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="8d01a-105">Útmutatónk biztosítja a küldő hitelesítését (ellenőrzi, hogy a küldő tartomány nem kerül hamisításra).</span><span class="sxs-lookup"><span data-stu-id="8d01a-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="8d01a-106">**Megjegyzés:** Nem javasoljuk a hamis pozitív adatok biztonságos feladói listák használatával történő kezelését, mivel a levélszemétszűrés alóli kivételek megnyithatják a szervezetet a biztonsági támadások előtt.</span><span class="sxs-lookup"><span data-stu-id="8d01a-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="8d01a-107">Ha a felhasználó(k) olyan üzeneteket kapnak, amelyek helytelenül spamként vagy levélszemétként vannak megjelölve, kérjük, **[jelentsék az üzeneteket és fájlokat a Microsoftnak.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="8d01a-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="8d01a-108">**Kerülni kell** a megbízható feladókat az Outlook ban, az Engedélyezett feladók listáját vagy a levélszemét-ellenes házirendekben engedélyezett tartománylistát, mivel a feladók megkerülik az összes levélszemét-, hamisítás- és adathalászat-védelmet, valamint a feladó hitelesítését (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="8d01a-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="8d01a-109">Ez a módszer csak ideiglenes tesztelésre használható.</span><span class="sxs-lookup"><span data-stu-id="8d01a-109">This method is best used for temporary testing only.</span></span>
