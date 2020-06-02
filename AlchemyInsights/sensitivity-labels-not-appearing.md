---
title: Nem megjelenő érzékenységi címkék
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 1326eca02044014a8e9c072fcc3e4cd3a41c7a9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511654"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="70743-102">Nem megjelenő érzékenységi címkék</span><span class="sxs-lookup"><span data-stu-id="70743-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="70743-103">Az érzékenységi címkék lehetővé teszik az érzékeny tartalmak osztályozását és védelmét.</span><span class="sxs-lookup"><span data-stu-id="70743-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="70743-104">Ezek a Microsoft 365 megfelelőségi központban, a Microsoft 365 biztonsági központban vagy a Microsoft 365 biztonsági & megfelelőségi központban hozhatók létre a Besorolási > az érzékenységi címkék alatt.</span><span class="sxs-lookup"><span data-stu-id="70743-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="70743-105">A funkcióról az [Érzékenységi címkék áttekintése című témakörben olvashat bővebben.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)</span><span class="sxs-lookup"><span data-stu-id="70743-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="70743-106">Ha konfigurálta az érzékenységi címkéket, de azok nem jelennek meg az Office-alkalmazásokban, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="70743-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="70743-107">Ellenőrizze, hogy az érzékenységi címke [közzé lett-e téve](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) a kívánt felhasználók és csoportok számára.</span><span class="sxs-lookup"><span data-stu-id="70743-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="70743-108">Ellenőrizze, hogy a felhasználó olyan alkalmazást használ-e, amely támogatja az érzékenységi címkéket – tekintse meg [az érzékenységi címkéket a dokumentumban.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)</span><span class="sxs-lookup"><span data-stu-id="70743-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="70743-109">Ha az [Azure Information Protection címkéket telepíti át,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)vegye figyelembe az [itt](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)felsorolt szempontokat.</span><span class="sxs-lookup"><span data-stu-id="70743-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="70743-110">Adatveszteség-megelőzési (DLP) támogatás: Jelenleg csak a megőrzési címkék használhatók feltételként a DLP-házirendekben.</span><span class="sxs-lookup"><span data-stu-id="70743-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="70743-111">A DLP-házirendben az érzékenységi címkék támogatása még nem érhető el, de dolgozunk rajta.</span><span class="sxs-lookup"><span data-stu-id="70743-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="70743-112">Ha a titkosítás engedélyezve van egy érzékenységi címkén, a következő t választhatja:</span><span class="sxs-lookup"><span data-stu-id="70743-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="70743-113">Engedélyek hozzárendelése most</span><span class="sxs-lookup"><span data-stu-id="70743-113">Assign permissions now</span></span>
    - <span data-ttu-id="70743-114">Engedélyek hozzárendelésének lehetővé teszi a felhasználók számára</span><span class="sxs-lookup"><span data-stu-id="70743-114">Let users assign permissions</span></span>


<span data-ttu-id="70743-115">A lehetséges problémákról az [Ismert érzékenységi címkékkel kapcsolatos tudnivalók](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="70743-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>