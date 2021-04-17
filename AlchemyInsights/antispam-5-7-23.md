---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821413"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="24b01-102">Az 5.7.23-as hibakódos levélk kézbesítési problémáinak megoldása</span><span class="sxs-lookup"><span data-stu-id="24b01-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="24b01-103">Ellenőrizze tartománya SPF DNS-rekordját egy nyilvánosan elérhető SPF vagy DNS-rekord-ellenőrző segítségével az interneten.</span><span class="sxs-lookup"><span data-stu-id="24b01-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="24b01-104">Győződjön meg arról, hogy a kimenő üzenetet nem azonosította levélszemétként a Microsoft, és az üzenetet a Magas kockázatú kézbesítési [készleten keresztül kézbesíti.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="24b01-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="24b01-105">A Magas kockázatú kézbesítési készletbe küldött üzenetek nem fognak átesni az SPF-ellenőrzéseken, ezért a cél levelezési szervezet nem fogadja el őket.</span><span class="sxs-lookup"><span data-stu-id="24b01-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="24b01-106">Ha a probléma nem szűnik meg, előfordulhat, hogy kapcsolatba kell lépnie annak a levelezési szolgáltatónak a rendszergazdával, amelybe e-mailt próbál küldeni.</span><span class="sxs-lookup"><span data-stu-id="24b01-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="24b01-107">Jegyezze fel a visszapattanó üzenetben elérhető részletes külső hibát.</span><span class="sxs-lookup"><span data-stu-id="24b01-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="24b01-108">Előfordulhat, hogy a Microsoft ügyfélszolgálata nem tud további segítséget nyújtani.</span><span class="sxs-lookup"><span data-stu-id="24b01-108">Microsoft support may not be able to assist further.</span></span>
