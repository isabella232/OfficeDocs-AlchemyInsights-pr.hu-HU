---
title: Feltételes hozzáférés Intune-nal
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704788"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c584c-102">Feltételes hozzáférés Intune-nal</span><span class="sxs-lookup"><span data-stu-id="c584c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c584c-103">A  **feltételes hozzáférés**  Intune-nal való használatához 3 lépés szükséges:</span><span class="sxs-lookup"><span data-stu-id="c584c-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="c584c-104">Megfelelőségi  **szabályzat** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)és  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)segítségével megadhatja azokat a beállításokat, amelyeknek teljesülnie kell ahhoz, hogy az eszköz megfelelőnek minősül.</span><span class="sxs-lookup"><span data-stu-id="c584c-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c584c-105">Egy eszköznek például legalább 6 jegyű pin-kódot kell lennie, mielőtt megfelelőnek minősül.</span><span class="sxs-lookup"><span data-stu-id="c584c-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="c584c-106">Hozzon létre **egy feltételes**  hozzáférési házirendet, amely meghatározza, hogy milyen erőforrások vannak védve, és milyen feltételeknek kell teljesülni az erőforrások eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="c584c-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="c584c-107">[Egy eszköznek például](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  kompatibilisnek kell lennie a vállalati e-mailek elérése előtt.</span><span class="sxs-lookup"><span data-stu-id="c584c-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="c584c-108">Győződjön meg **arról, hogy a megfelelőségi szabályzatok**  és  **a**  feltételes hozzáférési szabályzatok a kívánt felhasználócsoportokra vannak megcélzottak.</span><span class="sxs-lookup"><span data-stu-id="c584c-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="c584c-109">Ehhez szükség lehet bizonyos felhasználói csoportok létrehozására az Azure Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="c584c-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="c584c-110">**Hasznos hivatkozások:**</span><span class="sxs-lookup"><span data-stu-id="c584c-110">**Helpful links:**</span></span>

[<span data-ttu-id="c584c-111">Eszköz-megfelelőség áttekintése</span><span class="sxs-lookup"><span data-stu-id="c584c-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="c584c-112">A hitelesítésszolgáltató hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="c584c-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="c584c-113">Hibaelhárítási házirend</span><span class="sxs-lookup"><span data-stu-id="c584c-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="c584c-114">Az e-mailek (Exchange Online) nem kompatibilis eszközök által való elérésének védelme érdekében mindkét dokumentumot követnie kell:</span><span class="sxs-lookup"><span data-stu-id="c584c-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="c584c-115">Az e-mailek elérésének védelme az eszközökről az EAS használatával</span><span class="sxs-lookup"><span data-stu-id="c584c-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="c584c-116">Az e-mail-hozzáférés védelme az eszközökről modern hitelesítési ügyfélprogramokkal, például az Outlookkal</span><span class="sxs-lookup"><span data-stu-id="c584c-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)