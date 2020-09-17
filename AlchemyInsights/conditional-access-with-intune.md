---
title: Feltételes hozzáférés a Intune szolgáltatással
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807661"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f93a7-102">Feltételes hozzáférés a Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="f93a7-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f93a7-103">A  **feltételes hozzáférés**  használata a Intune használatához 3 lépésből áll:</span><span class="sxs-lookup"><span data-stu-id="f93a7-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="f93a7-104">Hozzon létre egy  **megfelelőségi házirendet**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) a megfelelő beállítások megadásához, mielőtt az eszköz megfelel-e a követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="f93a7-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="f93a7-105">Az eszközöknek például legalább 6 számjegyből álló PIN-kóddal kell rendelkezniük ahhoz, hogy megfeleljenek a megfelelőségi követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="f93a7-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="f93a7-106">Hozzon létre egy **feltételes hozzáférési házirendet**  , amely meghatározza, hogy milyen erőforrások legyenek védve, és milyen feltételeknek kell teljesülniük ahhoz, hogy hozzáférhessenek ezekhez az erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="f93a7-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="f93a7-107">[Az](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  eszközöknek például kompatibiliseknek kell lenniük a vállalati e-mailek eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="f93a7-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="f93a7-108">Gondoskodjon arról, hogy a **megfelelőségi szabályok**  és a  **feltételes hozzáférés-házirendek**  a felhasználók kívánt csoportjaira irányuljanak.</span><span class="sxs-lookup"><span data-stu-id="f93a7-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="f93a7-109">Ehhez szükség lehet az Azure Active Directory-beli felhasználók bizonyos csoportjai létrehozására.</span><span class="sxs-lookup"><span data-stu-id="f93a7-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="f93a7-110">**Hasznos hivatkozások:**</span><span class="sxs-lookup"><span data-stu-id="f93a7-110">**Helpful links:**</span></span>

[<span data-ttu-id="f93a7-111">Az eszközök megfelelősége – áttekintés</span><span class="sxs-lookup"><span data-stu-id="f93a7-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f93a7-112">HITELESÍTÉSSZOLGÁLTATÓ hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="f93a7-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f93a7-113">Hibaelhárítási szabályok</span><span class="sxs-lookup"><span data-stu-id="f93a7-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="f93a7-114">Ha nem kompatibilis eszközökről szeretné megvédeni az e-maileket (Exchange Online), mindkét dokumentumot meg kell tartani:</span><span class="sxs-lookup"><span data-stu-id="f93a7-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="f93a7-115">E-mail-hozzáférés védelme az eszközökről az EAS segítségével</span><span class="sxs-lookup"><span data-stu-id="f93a7-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="f93a7-116">E-mail-hozzáférés biztosítása az eszközökről a modern hitelesítési ügyfélprogramokkal (például az Outlookkal)</span><span class="sxs-lookup"><span data-stu-id="f93a7-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)