---
title: Javasolt lépések egy fiók feltörése esetén
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: 08904708dd19104179c3f97f6734d8af725a4512
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745435"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="3b04f-102">Javasolt lépések egy fiók feltörése esetén</span><span class="sxs-lookup"><span data-stu-id="3b04f-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="3b04f-103">VIDEÓ: Feltört Office 365-fiók helyreállítása</span><span class="sxs-lookup"><span data-stu-id="3b04f-103">VIDEO: Fixing a compromised Office 365 account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="3b04f-104">Azonnal [állítson be új jelszót a felhasználónak](https://docs.microsoft.com/office365/admin/add-users/reset-passwords).</span><span class="sxs-lookup"><span data-stu-id="3b04f-104">[Reset the user's password](https://docs.microsoft.com/office365/admin/add-users/reset-passwords) immediately.</span></span> <span data-ttu-id="3b04f-105">Ne küldje el e-mailben az új jelszót a végfelhasználónak.</span><span class="sxs-lookup"><span data-stu-id="3b04f-105">Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="3b04f-106">Távolítson el minden gyanús, a postaláda szintjén megadott [továbbítási címet](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="3b04f-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="3b04f-107">Távolítson el minden gyanús, a postaládában megadott [levelezési szabályt](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED).</span><span class="sxs-lookup"><span data-stu-id="3b04f-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="3b04f-108">Ha a felhasználónak meg van tiltva az e-mailek küldése, nyissa meg a [Korlátozott jogú felhasználók lapot, és oldja fel a fiók zárolását](https://protection.office.com/?hash=/restrictedusers).</span><span class="sxs-lookup"><span data-stu-id="3b04f-108">If the user is blocked from sending email, [go to the Restricted Users to unblock the account](https://protection.office.com/?hash=/restrictedusers).</span></span> <span data-ttu-id="3b04f-109">Ezt követően a felhasználónak egy órán belül ismét el kell tudnia küldeni az üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="3b04f-109">Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="3b04f-110">Távolítsa el a fiókot minden [rendszergazdai szerepkörű csoportból](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles), amíg meg nem győződik arról, hogy a fiókot sikerült helyreállítani.</span><span class="sxs-lookup"><span data-stu-id="3b04f-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="3b04f-111">Az adatokkal való jövőbeli visszaélések vagy a fiókok feltörésének minimalizálása érdekében azt javasoljuk, hogy olvassa el az [Office 365 biztonsági ütemtervet ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span><span class="sxs-lookup"><span data-stu-id="3b04f-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Office 365 Security best practices article](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  