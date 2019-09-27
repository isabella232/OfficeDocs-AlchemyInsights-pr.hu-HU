---
title: A érzékenységi címkék nem jelennek meg
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207227"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="a13f9-102">A érzékenységi címkék nem jelennek meg</span><span class="sxs-lookup"><span data-stu-id="a13f9-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="a13f9-103">A érzékenységi címkék lehetővé teszik a kényes tartalmak osztályozását és védelmét.</span><span class="sxs-lookup"><span data-stu-id="a13f9-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="a13f9-104">Ők lehet teremtett-ban Mikroszkóp 365 engedékenység központ, Mikroszkóp 365 Biztonság Központ, vagy hivatal 365 biztonság & engedékenység központ alatt osztályozás > érzékenység felirat.</span><span class="sxs-lookup"><span data-stu-id="a13f9-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="a13f9-105">A szolgáltatásról az [érzékenységi címkék áttekintése](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)című témakör nyújt bővebb felvilágosítást.</span><span class="sxs-lookup"><span data-stu-id="a13f9-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="a13f9-106">Ha beállította az érzékenységi címkéket, de azok nem jelennek meg az Office-alkalmazásokban, ellenőrizze a következőket:</span><span class="sxs-lookup"><span data-stu-id="a13f9-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="a13f9-107">Győződjön meg arról, hogy az érzékenységi címkét a kívánt felhasználók és csoportok számára [közzétették](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) .</span><span class="sxs-lookup"><span data-stu-id="a13f9-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="a13f9-108">Ellenőrizze, hogy a felhasználó használ-e olyan alkalmazást, amely támogatja a érzékenységi címkéket – lásd: [érzékenységi címkék a dokumentumban](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="a13f9-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="a13f9-109">Ha [áttelepíti a Azure adatvédelmet](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), vegye figyelembe az [itt](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)felsorolt szempontokat.</span><span class="sxs-lookup"><span data-stu-id="a13f9-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="a13f9-110">Adatvesztés megelőzése (DLP) támogatás: jelenleg csak az adatmegőrzési címkéket lehet használni a DLP-házirendek feltételeként.</span><span class="sxs-lookup"><span data-stu-id="a13f9-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="a13f9-111">A DLP-házirend érzékenységi címkéinek támogatása még nem érhető el, de rajta dolgozunk.</span><span class="sxs-lookup"><span data-stu-id="a13f9-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="a13f9-112">Ha egy érzékenységi címkén engedélyezve van a titkosítás, az alábbiak közül választhat:</span><span class="sxs-lookup"><span data-stu-id="a13f9-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="a13f9-113">Engedélyek hozzárendelése most</span><span class="sxs-lookup"><span data-stu-id="a13f9-113">Assign permissions now</span></span>
    - <span data-ttu-id="a13f9-114">A felhasználók hozzárendeljék az engedélyeket</span><span class="sxs-lookup"><span data-stu-id="a13f9-114">Let users assign permissions</span></span>


<span data-ttu-id="a13f9-115">A lehetséges problémákról további információt a [érzékenységi címkékkel kapcsolatos ismert problémák](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="a13f9-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>