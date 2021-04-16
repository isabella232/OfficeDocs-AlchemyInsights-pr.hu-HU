---
title: Meg kell jelölnie egy tartomány vagy e-mail feladóját?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792134"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="1d5fc-102">Meg kell jelölnie egy tartomány vagy e-mail feladóját?</span><span class="sxs-lookup"><span data-stu-id="1d5fc-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="1d5fc-103">A megbízható **feladók** listájának használata nem ajánlott, mivel a szervezetet levélszemét, adatszemét és hamisítási támadások ellen nyitja meg.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="1d5fc-104">Ha azonban van üzleti követelmény, azt javasoljuk, **hogy** ehhez az **[e-mail-forgalomra](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** vonatkozó szabályokat használja.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="1d5fc-105">Útmutatásunk biztosítja a feladók hitelesítését (ellenőrzi, hogy a küldő tartományt nem hamis használják-e fel).</span><span class="sxs-lookup"><span data-stu-id="1d5fc-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="1d5fc-106">**Megjegyzés:** Nem javasoljuk a vak pozitív üzenetek biztonságos feladók listákkal való kezelésének alkalmazását, mert a levélszemétszűrés alóli kivételek megnyitják szervezetét a biztonsági támadások ellen.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="1d5fc-107">Ha a felhasználó(k) helytelenül levélszemétként vagy levélszemétként megjelölt üzeneteket kapnak, kérjük, jelentse az üzeneteket és fájlokat a **[Microsoftnak.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="1d5fc-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="1d5fc-108">Az Outlook megbízható feladói, az engedélyezett feladók listája  és az engedélyezett tartománylista a levélszemét-szűrési házirendek során kerülendő, mert a feladók megkerülik az összes levélszemét, hamisítás és adatvédelmet, valamint a feladók hitelesítését (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="1d5fc-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="1d5fc-109">Ez a módszer csak ideiglenes teszteléshez ajánlott.</span><span class="sxs-lookup"><span data-stu-id="1d5fc-109">This method is best used for temporary testing only.</span></span>
