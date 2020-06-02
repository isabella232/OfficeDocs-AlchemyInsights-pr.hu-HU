---
title: 'AIP: A házirendek nem a várt módon viselkednek'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493158"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="e476a-102">AIP: A házirendek nem a várt módon viselkednek</span><span class="sxs-lookup"><span data-stu-id="e476a-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="e476a-103">Azure Information Protection: Szabályzatok nem viselkednek a várt módon, lásd a következő ajánlott irányelvek különböző szabályzati problémák:</span><span class="sxs-lookup"><span data-stu-id="e476a-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="e476a-104">Ha vizuális jelölésekkel kapcsolatos problémái vannak, kérjük, olvassa el [A vizuális jelölések alkalmazásakor való áttekintést.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="e476a-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="e476a-105">Ha problémái vannak az automatikus címkézéssel, tekintse át a [Hogyan konfigurálhatja az Azure Information Protection automatikus és ajánlott besorolási feltételeit,](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) és [hogy milyen bizalmas információtípusokat keresnek.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e476a-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="e476a-106">Ha problémákat okoz a Ninatív/Pfile-védelemmel, tekintse át [a Fájl API-konfigurációját.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="e476a-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="e476a-107">Ellenőrizze, hogy olyan hatókörrel kapcsolatos szabályzatokat használ-e, amelyek nincsenek megfelelően konfigurálva: [Az Azure Information Protection szabályzat konfigurálása adott felhasználók számára hatókörrel kapcsolatos szabályzatok használatával.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="e476a-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="e476a-108">Ha az automatikus címkézés nem működik az Outlook programban, amikor címkézett dokumentumot csatol, ellenőrizze, hogy a DRMEncryptProperty nincs-e definiálva az itt leírtak szerint: [Tartalomvédelmi rendszerbiztonsági beállításjegyzék-beállítások](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="e476a-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="e476a-109">Ha továbbra is problémákat tapasztal, gyűjtse össze az Azure Information Protection ügyfélnaplókat, és csatolja az exportált naplókat ehhez a jegyhez.</span><span class="sxs-lookup"><span data-stu-id="e476a-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="e476a-110">Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="e476a-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="e476a-111">Kattintson **a Védelem/érzékenység**  >  **súgó és visszajelzés gombra.**</span><span class="sxs-lookup"><span data-stu-id="e476a-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="e476a-112">Kattintson **a Naplók exportálása gombra.**</span><span class="sxs-lookup"><span data-stu-id="e476a-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="e476a-113">Mentse a naplókat a választott helyre, és csatolja őket ehhez a szolgáltatási kérelemhez.</span><span class="sxs-lookup"><span data-stu-id="e476a-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="e476a-114">További források:</span><span class="sxs-lookup"><span data-stu-id="e476a-114">Additional resources:</span></span>

- [<span data-ttu-id="e476a-115">Az Azure Information Protection vizuális jelölései címkéjének konfigurálása</span><span class="sxs-lookup"><span data-stu-id="e476a-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="e476a-116">Tekintse át az Azure Information Protection dokumentációját</span><span class="sxs-lookup"><span data-stu-id="e476a-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="e476a-117">Érzékenységi címkék használata az Office-appokban</span><span class="sxs-lookup"><span data-stu-id="e476a-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

