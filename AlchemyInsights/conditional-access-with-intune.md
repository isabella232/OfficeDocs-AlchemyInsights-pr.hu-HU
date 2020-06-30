---
title: Feltételes hozzáférés az Intune-nal
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931434"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b6b78-102">Feltételes hozzáférés az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="b6b78-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b6b78-103">A **feltételes hozzáférés** intune-nal való használata 3 lépést igényel:</span><span class="sxs-lookup"><span data-stu-id="b6b78-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="b6b78-104">Hozzon létre **megfelelőségi szabályzatot** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) olyan beállítások meghatározásához, amelyeknek meg kell felelniük ahhoz, hogy az eszköz megfelelőnek minősüljen.</span><span class="sxs-lookup"><span data-stu-id="b6b78-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b6b78-105">Egy eszköznek például legalább 6 számjegyből álló tűvel kell rendelkeznie ahhoz, hogy megfelelőnek minősüljön.</span><span class="sxs-lookup"><span data-stu-id="b6b78-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="b6b78-106">Hozzon létre egy **feltételes hozzáférési szabályzatot,** amely meghatározza, hogy milyen erőforrások at védenek, és milyen feltételeknek kell megfelelni az erőforrások eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="b6b78-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="b6b78-107">Egy eszköznek [például](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) megfelelőnek kell lennie a vállalati e-mailek elérése előtt.</span><span class="sxs-lookup"><span data-stu-id="b6b78-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="b6b78-108">Győződjön meg arról, hogy mind **a megfelelőségi szabályzatok,** mind a **feltételes hozzáférési házirendek** a kívánt felhasználói csoportokat célozzák meg.</span><span class="sxs-lookup"><span data-stu-id="b6b78-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="b6b78-109">Ez szükség lehet a felhasználók adott csoportjainak az Azure Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="b6b78-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="b6b78-110">**Hasznos linkek:**</span><span class="sxs-lookup"><span data-stu-id="b6b78-110">**Helpful links:**</span></span>

[<span data-ttu-id="b6b78-111">Eszközmegfelelőség – áttekintés</span><span class="sxs-lookup"><span data-stu-id="b6b78-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="b6b78-112">Hitelesítésak – hibaelhárítás</span><span class="sxs-lookup"><span data-stu-id="b6b78-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b6b78-113">Hibaelhárítási házirend</span><span class="sxs-lookup"><span data-stu-id="b6b78-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="b6b78-114">Annak érdekében, hogy az e-maileket (Exchange online) megvédje a nem megfelelő eszközök hozzáférésétől, mindkét dokumentumot be kell tartani:</span><span class="sxs-lookup"><span data-stu-id="b6b78-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="b6b78-115">Az e-mailek elérésének védelme az eszközökről az EAS használatával</span><span class="sxs-lookup"><span data-stu-id="b6b78-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="b6b78-116">Az e-mailek elérésének védelme az eszközökkel a modern hitelesítési ügyfelek, például az Outlook használatával</span><span class="sxs-lookup"><span data-stu-id="b6b78-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)