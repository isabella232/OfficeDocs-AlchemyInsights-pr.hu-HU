---
title: 'AIP: A házirendek nem a várt módon viselkednek'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821629"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="9209d-102">AIP: A házirendek nem a várt módon viselkednek</span><span class="sxs-lookup"><span data-stu-id="9209d-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="9209d-103">Azure Information Protection: A házirendek nem a várt módon viselkednek. A különböző házirendekkel kapcsolatos problémákhoz az alábbi ajánlott irányelveket ajánljuk:</span><span class="sxs-lookup"><span data-stu-id="9209d-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="9209d-104">Ha problémákat jelentkezik a vizuális jelölésekkel kapcsolatban, kérjük, olvassa el a Vizuális [jelölések alkalmazásakor.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="9209d-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="9209d-105">Ha problémákat okozhat az automatikus címkézéssel kapcsolatban, olvassa el a Feltételek konfigurálása az [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) automatikus és ajánlott besorolásához és A bizalmas [adattípusok által keresnek.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="9209d-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="9209d-106">Ha natív/Pfile protection-problémákat jelentkezik, tekintse át a [Fájl API-konfigurációt.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="9209d-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="9209d-107">Ellenőrizze, hogy nem megfelelően konfigurált hatókörű házirendeket használ-e: Az Azure Information Protection házirend konfigurálása adott felhasználók számára hatókörű [házirendek használatával.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="9209d-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="9209d-108">Ha az Outlookban nem működik az automatikus feliratozás, amikor címkével jelölt dokumentumot csatol, ellenőrizze, hogy a DRMEncryptProperty nincs-e definiálva a következő módon: [Biztonsági tartalomvédelmi beállításjegyzék-beállítások.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="9209d-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="9209d-109">Ha továbbra is problémákat tapasztal, gyűjtse össze az Azure Information Protection-ügyfélnaplókat, és csatolja az exportált naplókat ehhez a jegyhez.</span><span class="sxs-lookup"><span data-stu-id="9209d-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="9209d-110">Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="9209d-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="9209d-111">Kattintson **a Védelem/bizalmasság – súgó** és visszajelzés  >  **elemre.**</span><span class="sxs-lookup"><span data-stu-id="9209d-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="9209d-112">Kattintson **a Naplók exportálása elemre.**</span><span class="sxs-lookup"><span data-stu-id="9209d-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="9209d-113">Mentse a naplókat a választott helyre, és csatolja őket ehhez a szolgáltatáskéréshez.</span><span class="sxs-lookup"><span data-stu-id="9209d-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="9209d-114">További források:</span><span class="sxs-lookup"><span data-stu-id="9209d-114">Additional resources:</span></span>

- [<span data-ttu-id="9209d-115">Címke beállítása vizuális jelöléshez az Azure Information Protectionben</span><span class="sxs-lookup"><span data-stu-id="9209d-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="9209d-116">Az Azure Information Protection dokumentációjának áttekintése</span><span class="sxs-lookup"><span data-stu-id="9209d-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="9209d-117">Bizalmasság-címkék használata a Microsoft 365-ös alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="9209d-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

