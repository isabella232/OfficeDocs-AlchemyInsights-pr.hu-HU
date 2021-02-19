---
title: A felhasználók kártékony e-mailt kaptak?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291794"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="cccaa-102">A felhasználók kártékony e-mailt kaptak?</span><span class="sxs-lookup"><span data-stu-id="cccaa-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="cccaa-103">Mostantól bejelentheti a kártékony e-maileket a Microsoftnak a [Biztonsági és megfelelőségi központ Adminisztrátorok által beküldött elemek területén](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="cccaa-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="cccaa-104">Az [Adminisztrátorok által beküldött elemek](https://sip.protection.office.com/reportsubmission) között beküldött üzeneteket megvizsgáljuk, és az alábbi eredményeknek kell megjelenniük a **Részletek** előugró panelen:</span><span class="sxs-lookup"><span data-stu-id="cccaa-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="cccaa-105">Történt-e hiba a küldő e-mailjének hitelesítésekor az üzenet kézbesítése során.</span><span class="sxs-lookup"><span data-stu-id="cccaa-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="cccaa-106">Tájékoztatás azokról a házirendnek való megfelelésekről, amelyek befolyásolhatták vagy felülbírálhatták az üzenetre vonatkozó biztonsági rendelkezést.</span><span class="sxs-lookup"><span data-stu-id="cccaa-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="cccaa-107">Az aktuális hatástalanítási eredmények, amelyekből megállapítható, hogy az üzenetben szereplő URL-címek vagy fájlok kártékonyak voltak-e, vagy sem.</span><span class="sxs-lookup"><span data-stu-id="cccaa-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="cccaa-108">Visszajelzés az osztályozóktól</span><span class="sxs-lookup"><span data-stu-id="cccaa-108">Feedback from graders</span></span>

<span data-ttu-id="cccaa-109">Felülbírálás esetén az újbóli vizsgálatnak néhány perc alatt be kell fejeződnie.</span><span class="sxs-lookup"><span data-stu-id="cccaa-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="cccaa-110">Ha nem volt probléma az e-mail hitelesítése során, vagy ha nem befolyásolta felülbírálás a kézbesítést, az osztályozóktól kapott visszajelzésre akár egy napot is várnia kellhet.</span><span class="sxs-lookup"><span data-stu-id="cccaa-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="cccaa-111">Ha nem ért egyet egy üzenetre, URL-címre vagy fájlra vonatkozó végső biztonsági rendelkezéssel (letiltva vagy nem letiltva), egy nap múlva küldje el újra az üzenetet újbóli vizsgálatra.</span><span class="sxs-lookup"><span data-stu-id="cccaa-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="cccaa-112">Az üzenet újbóli beküldése után a biztonsági rendelkezés nagy valószínűséggel megváltozik majd.</span><span class="sxs-lookup"><span data-stu-id="cccaa-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="cccaa-113">Eközben az [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) olvasható utasításokat követve eltávolíthatja a kártékony e-maileket a felhasználók postaládájából.</span><span class="sxs-lookup"><span data-stu-id="cccaa-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="cccaa-114">Az Office 365-höz készült Microsoft Defendert használó ügyfeleknek a következőkre nyílik lehetőségük:</span><span class="sxs-lookup"><span data-stu-id="cccaa-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="cccaa-115">A [Veszélyforrás-felderítővel megkereshetik és törölhetik a gyanús e-maileket](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered).</span><span class="sxs-lookup"><span data-stu-id="cccaa-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="cccaa-116">A [Biztonságos hivatkozások funkcióval letilthatják a hozzáférést](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a kártékony URL-címekhez.</span><span class="sxs-lookup"><span data-stu-id="cccaa-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="cccaa-117">Nyomon követhetik a kártékony URL-címre kattintó és azt megnyitó felhasználókat: [Megtekinthetik az adathalász URL-címek és kattintási biztonsági rendelkezések adatait](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace).</span><span class="sxs-lookup"><span data-stu-id="cccaa-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="cccaa-118">Manuálisan [elindíthatnak egy automatizált vizsgálatot](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).</span><span class="sxs-lookup"><span data-stu-id="cccaa-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="cccaa-119">A [Védelem a kártékony URL-címekkel és fájlokkal szemben](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) című témakörben leírt utasításokat követve is biztosíthatja a kártékony fájlokkal és URL-címekkel szembeni védelmet.</span><span class="sxs-lookup"><span data-stu-id="cccaa-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>