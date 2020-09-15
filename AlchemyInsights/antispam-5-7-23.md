---
title: Antispam-5.7.23 hibakódú
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717327"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="51f6d-102">Az e-mailek kézbesítésével kapcsolatos problémák megoldása a hibakódok 5.7.23 hibakódú</span><span class="sxs-lookup"><span data-stu-id="51f6d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="51f6d-103">Ellenőrizze a tartomány SPF DNS-rekordját a nyilvánosan elérhető SPF-vagy DNS-rekordok ellenőrzésekor a weben.</span><span class="sxs-lookup"><span data-stu-id="51f6d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="51f6d-104">Ellenőrizze, hogy a kimenő üzenet a Microsofttól kapott-e levélszemétként, és a [nagy kockázatú kézbesítési készleten](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)keresztül továbbítódik-e.</span><span class="sxs-lookup"><span data-stu-id="51f6d-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="51f6d-105">A magas kockázatú kézbesítési készlet üzenetei nem jutnak el az SPF-ellenőrzésekhez, ezért a cél e-mail-szervezet nem fogadja el őket.</span><span class="sxs-lookup"><span data-stu-id="51f6d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="51f6d-106">Ha a probléma nem szűnik meg, előfordulhat, hogy fel kell vennie a figyelmét annak a levelezési állomásnak a rendszergazdájára, amelyhez e-mailt próbál küldeni.</span><span class="sxs-lookup"><span data-stu-id="51f6d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="51f6d-107">Jegyezze fel a visszafordulási üzenetben elérhető részletes külső hibát.</span><span class="sxs-lookup"><span data-stu-id="51f6d-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="51f6d-108">Előfordulhat, hogy a Microsoft ügyfélszolgálata nem tud további segítséget nyújtani.</span><span class="sxs-lookup"><span data-stu-id="51f6d-108">Microsoft support may not be able to assist further.</span></span>
