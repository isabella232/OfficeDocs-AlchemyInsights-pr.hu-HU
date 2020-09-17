---
title: Biztonságosnak kell lennie egy tartománynak vagy egy e-mail-feladónak?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803247"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="fead9-102">Biztonságosnak kell lennie egy tartománynak vagy egy e-mail-feladónak?</span><span class="sxs-lookup"><span data-stu-id="fead9-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="fead9-103">A **megbízható küldők listái nem ajánlottak** , mivel a szervezetet a levélszemét, az adathalász és a hamisítás elleni támadások megadásával nyitják meg.</span><span class="sxs-lookup"><span data-stu-id="fead9-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="fead9-104">Ha azonban üzleti szükséglete van, azt **javasoljuk** , hogy e- **[mail-forgalom szabályait](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** használja ehhez a szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="fead9-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="fead9-105">Útmutatásunk szerint a küldő tartomány hitelesítése (a küldő tartomány ellenőrzése nem hamisítható meg).</span><span class="sxs-lookup"><span data-stu-id="fead9-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="fead9-106">**Megjegyzés**: nem javasoljuk a téves pozitív adatok kezelését a megbízható küldők listáival, mert a levélszemét-szűrés alóli kivételek a szervezet biztonsági támadások számára való megnyitását szolgálják.</span><span class="sxs-lookup"><span data-stu-id="fead9-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="fead9-107">Ha a felhasználó (k) tévesen levélszemétként vagy levélszemétként megjelölt üzeneteket fogad, kérjük, jelezze **[az üzeneteket és a fájlokat a Microsoftnak](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="fead9-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="fead9-108">**Elkerülhetők** a megbízható feladók az Outlookban, az engedélyezett feladók vagy a megengedett tartományok listája a levélszemét elleni szabályokban, mivel a feladók megkerülik az összes levélszemét-, svindli-és adathalász-védelmet, valamint a feladó hitelesítését (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="fead9-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="fead9-109">Ezt a módszert a legjobb csak ideiglenes teszteléshez használja.</span><span class="sxs-lookup"><span data-stu-id="fead9-109">This method is best used for temporary testing only.</span></span>
