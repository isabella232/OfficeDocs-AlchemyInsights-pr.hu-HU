---
title: 'Rendszergazda: a házirendek nem a várt módon viselkednek.'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663191"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="4c42e-102">Rendszergazda: a házirendek nem a várt módon viselkednek.</span><span class="sxs-lookup"><span data-stu-id="4c42e-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="4c42e-103">Azure Information Protection: a házirendek a várttól eltérő módon működnek</span><span class="sxs-lookup"><span data-stu-id="4c42e-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="4c42e-104">Ha a vizuális jelzésekkel kapcsolatos problémákat tapasztal, olvassa el a [vizuális jelzések alkalmazása](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)esetén című témakört.</span><span class="sxs-lookup"><span data-stu-id="4c42e-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="4c42e-105">Ha problémák merülnek fel az automatikus címkézés során, kérjük, tekintse át, hogyan konfigurálhatja az Azure-alapú adatvédelem és [a bizalmas adattípusok](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) [automatikus és ajánlott besorolási feltételeit](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) .</span><span class="sxs-lookup"><span data-stu-id="4c42e-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="4c42e-106">Ha a natív/Pfile védelem során problémákat tapasztal, olvassa el a [fájlok API-konfigurációjának](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)áttekintése című témakört.</span><span class="sxs-lookup"><span data-stu-id="4c42e-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="4c42e-107">Ellenőrizze, hogy léteznek-e olyan hatókörű házirendek, amelyek nincs megfelelően konfigurálva: [Az Azure-adatvédelem házirendjének konfigurálása meghatározott felhasználókhoz hatóköres házirendek használatával](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="4c42e-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="4c42e-108">Ha a címkével ellátott dokumentumok csatolásakor az automatikus címkézés nem mûködik az Outlookban, ellenőrizze, hogy a DRMEncryptProperty nem az itt ismertetett módon van definiálva: [a tartalomvédelmi szolgáltatás beállításjegyzékének beállításai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="4c42e-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="4c42e-109">Ha továbbra is problémákat tapasztal, kérjük, gyűjtsön az Azure Information Protection ügyfél naplóit, és csatolja az exportált naplókat a jegyhez.</span><span class="sxs-lookup"><span data-stu-id="4c42e-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="4c42e-110">Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="4c42e-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="4c42e-111">Kattintson a **védelem/érzékenység**  >  **Súgó és visszajelzés**elemre.</span><span class="sxs-lookup"><span data-stu-id="4c42e-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="4c42e-112">Kattintson a **naplók exportálása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="4c42e-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="4c42e-113">Mentse a naplókat a kívánt helyre, és csatolja őket a szolgáltatási kéréshez.</span><span class="sxs-lookup"><span data-stu-id="4c42e-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="4c42e-114">További források:</span><span class="sxs-lookup"><span data-stu-id="4c42e-114">Additional resources:</span></span>

- [<span data-ttu-id="4c42e-115">Címke beállítása az Azure-védelemhez használható vizuális jelzésekhez</span><span class="sxs-lookup"><span data-stu-id="4c42e-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="4c42e-116">Az Azure Information Protection dokumentációjának áttekintése</span><span class="sxs-lookup"><span data-stu-id="4c42e-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="4c42e-117">Tartalmi címkék használata a Microsoft 365-alkalmazásokban</span><span class="sxs-lookup"><span data-stu-id="4c42e-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

