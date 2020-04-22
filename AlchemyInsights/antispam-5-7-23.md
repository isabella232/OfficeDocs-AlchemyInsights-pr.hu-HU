---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676499"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="b0e1f-102">Az 5.7.23-as hibakódú e-mailek kézbesítési problémáinak megoldása</span><span class="sxs-lookup"><span data-stu-id="b0e1f-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="b0e1f-103">Ellenőrizze a tartomány SPF DNS-rekordját egy nyilvánosan elérhető SPF- vagy DNS-rekordellenőrzőn az interneten.</span><span class="sxs-lookup"><span data-stu-id="b0e1f-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="b0e1f-104">Ellenőrizze, hogy a Microsoft nem azonosította-e a kimenő üzenetet levélszemétként, és nem jutott-e át a [magas kockázatú kézbesítési készleten.](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="b0e1f-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="b0e1f-105">A magas kockázatú kézbesítési készletben lévő üzenetek nem felelnek meg az SPF-ellenőrzéseknek, ezért a célleveles szervezet nem fogadja el őket.</span><span class="sxs-lookup"><span data-stu-id="b0e1f-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="b0e1f-106">Ha a probléma továbbra is fennáll, előfordulhat, hogy kapcsolatba kell lépnie annak a levélszolgáltatónak az adminjával, amelyiknek e-mailt próbál küldeni.</span><span class="sxs-lookup"><span data-stu-id="b0e1f-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="b0e1f-107">Jegyezze fel a részletes külső hibát a visszafordulási üzenetben.</span><span class="sxs-lookup"><span data-stu-id="b0e1f-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="b0e1f-108">Előfordulhat, hogy a Microsoft támogatási szolgálata nem tud további segítséget nyújtani.</span><span class="sxs-lookup"><span data-stu-id="b0e1f-108">Microsoft support may not be able to assist further.</span></span>
