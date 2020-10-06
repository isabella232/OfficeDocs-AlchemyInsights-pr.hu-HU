---
title: Feltételes hozzáférés figyelése
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366430"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="c2e01-102">Feltételes hozzáférés figyelése az Exchange-ben</span><span class="sxs-lookup"><span data-stu-id="c2e01-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="c2e01-103">A feltételes hozzáféréssel célzott felhasználók értesítést kapnak e-mailben, ha nem felelnek meg a szervezet hozzáférési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="c2e01-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="c2e01-104">A probléma megoldásához az alábbi megoldások közül legalább egyet ajánlunk:</span><span class="sxs-lookup"><span data-stu-id="c2e01-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="c2e01-105">Ha az eszköz feltételezetten regisztrált, értesítse a felhasználót, hogy nyissa meg a vállalati portál alkalmazást, és ellenőrizze, hogy megjelenik-e a vállalati portálon.</span><span class="sxs-lookup"><span data-stu-id="c2e01-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="c2e01-106">Ha nem, akkor a felhasználónak regisztrálnia kell az eszközt.</span><span class="sxs-lookup"><span data-stu-id="c2e01-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="c2e01-107">Az Azure portálon nyissa meg a Intune > eszköz megfelelősége című részt.</span><span class="sxs-lookup"><span data-stu-id="c2e01-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="c2e01-108">A monitor csoportban kattintson az eszköz megfelelősége elemre.</span><span class="sxs-lookup"><span data-stu-id="c2e01-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="c2e01-109">Tekintse meg az eszköz megfelelőségi jelentését annak ellenőrzéséhez, hogy a felhasználó eszközének megfelelően van-e megjelölve.</span><span class="sxs-lookup"><span data-stu-id="c2e01-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="c2e01-110">Az Azure portálon nyissa meg a Intune > eszköz megfelelősége című részt.</span><span class="sxs-lookup"><span data-stu-id="c2e01-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="c2e01-111">A kezelés csoportban kattintson a házirendek elemre.</span><span class="sxs-lookup"><span data-stu-id="c2e01-111">Under Manage, click Policies.</span></span> <span data-ttu-id="c2e01-112">Ellenőrizze, hogy a megfelelőségi házirendek listája tartalmazza-e a felhasználói eszközhöz tartozó profilt.</span><span class="sxs-lookup"><span data-stu-id="c2e01-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="c2e01-113">Ha nincs kiosztva profil, akkor a Intune nem fogja tudni ellenőrizni az eszköz megfelelőségi állapotát.</span><span class="sxs-lookup"><span data-stu-id="c2e01-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="c2e01-114">Módosítsa a felhasználó feltételes hozzáférés-hozzárendelését.</span><span class="sxs-lookup"><span data-stu-id="c2e01-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="c2e01-115">Az Azure portálon nyissa meg az **Intune**  >  **feltételes hozzáférési**  >  **házirendeket**.</span><span class="sxs-lookup"><span data-stu-id="c2e01-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="c2e01-116">Jelöljön ki egy házirendet a listából.</span><span class="sxs-lookup"><span data-stu-id="c2e01-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="c2e01-117">Kattintson a felhasználók és csoportok elemre.</span><span class="sxs-lookup"><span data-stu-id="c2e01-117">Click Users and groups.</span></span>
4. <span data-ttu-id="c2e01-118">Ha egy bizonyos házirendet valakinek szeretne célozni, vegye fel őket a belefoglalási listára.</span><span class="sxs-lookup"><span data-stu-id="c2e01-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="c2e01-119">Ha meg szeretne győződni arról, hogy egy személy nincs kihagyva a házirendből, vegye fel őket a kizárási listára.</span><span class="sxs-lookup"><span data-stu-id="c2e01-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="c2e01-120">Hasznos hivatkozások:</span><span class="sxs-lookup"><span data-stu-id="c2e01-120">Helpful links:</span></span>

[<span data-ttu-id="c2e01-121">Az eszközök megfelelősége – áttekintés</span><span class="sxs-lookup"><span data-stu-id="c2e01-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="c2e01-122">HITELESÍTÉSSZOLGÁLTATÓ hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="c2e01-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="c2e01-123">Hibaelhárítási szabályok</span><span class="sxs-lookup"><span data-stu-id="c2e01-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="c2e01-124">A Intune eszköz megfelelőségének figyelése</span><span class="sxs-lookup"><span data-stu-id="c2e01-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="c2e01-125">Megjegyzés: ezek a lépések csak az Azure Active Directory szolgáltatáshoz való feltételes hozzáférés hibaelhárításakor hasznosak.</span><span class="sxs-lookup"><span data-stu-id="c2e01-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="c2e01-126">Az is lehetséges, hogy egy eszköz karanténba helyezi az e-mail-hozzáférését az Exchange-házirenddel.</span><span class="sxs-lookup"><span data-stu-id="c2e01-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="c2e01-127">További információ az Exchange-eszközök kezeléséről [itt](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)található.</span><span class="sxs-lookup"><span data-stu-id="c2e01-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
