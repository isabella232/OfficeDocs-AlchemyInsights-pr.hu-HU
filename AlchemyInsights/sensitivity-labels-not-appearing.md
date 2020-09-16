---
title: Nem jelennek meg a tartalmi Címkék
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801186"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="f1aa1-102">Nem jelennek meg a tartalmi Címkék</span><span class="sxs-lookup"><span data-stu-id="f1aa1-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="f1aa1-103">A tartalmi címkék segítségével minősítheti és védheti a bizalmas tartalmakat.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="f1aa1-104">Ezek a Microsoft 365 megfelelőségi központban, a Microsoft 365 biztonsági központban vagy a Microsoft 365 biztonsági & megfelelőségi központban hozhatók létre > a tartalmi címkék osztályozása csoportban.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="f1aa1-105">A funkcióról a [tartalmi címkék áttekintése](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="f1aa1-106">Ha beállította a tartalmi címkéit, de nem jelennek meg a Microsoft 365-alkalmazásokban, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="f1aa1-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="f1aa1-107">Erősítse meg, hogy a tartalmi címkét [közzétették](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) a kívánt felhasználók és csoportok számára.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="f1aa1-108">Ellenőrizze, hogy a felhasználó egy olyan alkalmazást használ-e, amely támogatja a tartalmi címkéket – lásd: [a dokumentumban lévő tartalmi címkék](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="f1aa1-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="f1aa1-109">Ha Azure- [adatvédelemi címkéket szeretne áttelepíteni](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ügyeljen az [itt](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)ismertetett szempontokra.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="f1aa1-110">Adatveszteség-megelőzés (DLP) támogatása: jelenleg csak az adatmegőrzési címkék használhatók feltételként a DLP-házirendekben.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="f1aa1-111">Egy DLP-házirendben az érzékenységi címkék támogatása még nem érhető el, de éppen dolgozunk rajta.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="f1aa1-112">Ha a titkosítás engedélyezve van egy tartalmi címkén, az alábbiakra van lehetősége:</span><span class="sxs-lookup"><span data-stu-id="f1aa1-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="f1aa1-113">Engedélyek hozzárendelése most</span><span class="sxs-lookup"><span data-stu-id="f1aa1-113">Assign permissions now</span></span>
    - <span data-ttu-id="f1aa1-114">Engedélyek hozzárendelése a felhasználókhoz</span><span class="sxs-lookup"><span data-stu-id="f1aa1-114">Let users assign permissions</span></span>


<span data-ttu-id="f1aa1-115">A lehetséges problémákról további információt az [érzékenységi címkék ismert problémái](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="f1aa1-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>