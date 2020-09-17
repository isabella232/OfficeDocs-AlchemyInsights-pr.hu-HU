---
title: Tartalomhamisítást, adathalászatot vagy megszemélyesítést érintő problémák
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: 92e7f611b08a5457e52be248982785b2dc2ddabc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773021"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a><span data-ttu-id="2d52f-102">Tartalomhamisítást, adathalászatot vagy megszemélyesítést érintő problémák</span><span class="sxs-lookup"><span data-stu-id="2d52f-102">Issues with spoofing, phishing, or impersonation?</span></span>

<span data-ttu-id="2d52f-103">Ismerje meg, hogyan védi a Microsoft a következőket:</span><span class="sxs-lookup"><span data-stu-id="2d52f-103">Learn how Microsoft protects you from:</span></span>

- [<span data-ttu-id="2d52f-104">Svindli</span><span class="sxs-lookup"><span data-stu-id="2d52f-104">Spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)

- [<span data-ttu-id="2d52f-105">Adathalászat és megszemélyesítés</span><span class="sxs-lookup"><span data-stu-id="2d52f-105">Phishing and impersonation</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)

<span data-ttu-id="2d52f-106">További javaslatok:</span><span class="sxs-lookup"><span data-stu-id="2d52f-106">Additional recommendations:</span></span>

- <span data-ttu-id="2d52f-107">Abban az esetben, ha a hamisított feladók a saját tartományból származnak, az [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) és a [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) segíthetnek.</span><span class="sxs-lookup"><span data-stu-id="2d52f-107">For spoofed senders that appear to come from your own domain, [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) and [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) can help.</span></span>

- <span data-ttu-id="2d52f-108">Ellenőrizze, hogy a saját tartományában lévő feladók nincsenek-e bekapcsolva a levélszemét szűrésének mellőzésére a levelezési szabályok (más néven átviteli szabályok) vagy a listaelemek engedélyezése beállítással.</span><span class="sxs-lookup"><span data-stu-id="2d52f-108">Verify senders in your own domain aren't configured to bypass anti-spam filtering using mail flow rules (also known as transport rules) or allow list entries.</span></span> <span data-ttu-id="2d52f-109">További információt a figyelmeztetések a [Microsoft levélszemét-szűrők megkerülése ellen](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="2d52f-109">For more information, see [Cautions against bypassing Microsoft spam filters](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters).</span></span>

- <span data-ttu-id="2d52f-110">Ellenőrizze, hogy a felhasználók nem konfigurálták a [megbízható feladók listaelemeket](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) , amelyek lehetővé teszik az adathalászat elleni támadást.</span><span class="sxs-lookup"><span data-stu-id="2d52f-110">Verify that users haven't configured [Safe Senders list](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) entries that could allow phishing attacks.</span></span>

- <span data-ttu-id="2d52f-111">Fontolja meg a levélszemét és az adathalászati üzenetek karanténba helyezését a Levélszemét mappa helyett.</span><span class="sxs-lookup"><span data-stu-id="2d52f-111">Consider delivering high-confidence spam and phishing messages to quarantine instead of the Junk Email folder.</span></span> <span data-ttu-id="2d52f-112">További információt az [e-mail-üzenetek karanténba helyezése](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="2d52f-112">For more information, see [Quarantine email messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages).</span></span>

<span data-ttu-id="2d52f-113">**Az [üzenetek Microsoftnak való jelentése](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) a legjobb módszer arra, hogy tudassa velünk a szűrők végrehajtását.**</span><span class="sxs-lookup"><span data-stu-id="2d52f-113">**[Reporting messages to Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) is the best way to let us know how the filters are performing.**</span></span>
