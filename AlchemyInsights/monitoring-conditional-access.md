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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708676"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="d7bbd-102">Feltételes hozzáférés figyelése Exchange-hez</span><span class="sxs-lookup"><span data-stu-id="d7bbd-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="d7bbd-103">A feltételes hozzáféréssel megcélzott felhasználók értesítést kapnak e-mailben, ha nem teljesítik a szervezet hozzáférési követelményeit.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="d7bbd-104">A probléma megoldásához az alábbi megoldásokat javasoljuk:</span><span class="sxs-lookup"><span data-stu-id="d7bbd-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="d7bbd-105">Ha az eszköz regisztrálva van, javasolja a felhasználónak, hogy a Céges portál appban ellenőrizze, hogy megjelenik-e a céges portálon.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="d7bbd-106">Ha nem, a felhasználónak regisztrálnia kell az eszközt.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="d7bbd-107">Az Azure Portalon az Intune > eszköznek való megfelelőséghez.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="d7bbd-108">A Figyelés alatt kattintson az Eszköz megfelelősége elemre.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="d7bbd-109">Az eszköz megfelelőségi jelentésében ellenőrizheti, hogy a felhasználó eszköze kompatibilisként van-e megjelölve.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="d7bbd-110">Az Azure Portalon az Intune > eszköznek való megfelelőséghez.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="d7bbd-111">A Kezelés alatt kattintson a Házirendek elemre.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-111">Under Manage, click Policies.</span></span> <span data-ttu-id="d7bbd-112">A megfelelőségi szabályzatok listájában ellenőrizze, hogy van-e profil hozzárendelve a felhasználó eszközéhez.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="d7bbd-113">Ha nincs hozzárendelve profil, akkor az Intune nem fogja tudni megerősíteni az eszköz megfelelőségi állapotát.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="d7bbd-114">Szerkessze a felhasználó feltételes hozzáférési hozzárendelését.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="d7bbd-115">Az Azure Portalon az **Intune** feltételes hozzáférési  >  **szabályzatok**  >  **között.**</span><span class="sxs-lookup"><span data-stu-id="d7bbd-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="d7bbd-116">Válasszon egy házirendet a listából.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="d7bbd-117">Kattintson a Felhasználók és csoportok elemre.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-117">Click Users and groups.</span></span>
4. <span data-ttu-id="d7bbd-118">Ha meg szeretne adni egy házirendet valakinél, vegye fel a házirendet a Felvétel listára.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="d7bbd-119">Ha ki szeretne hagyni egy személyt a házirendből, vegye fel őket a Kizárás listára.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="d7bbd-120">Hasznos hivatkozások:</span><span class="sxs-lookup"><span data-stu-id="d7bbd-120">Helpful links:</span></span>

[<span data-ttu-id="d7bbd-121">Eszköz-megfelelőség áttekintése</span><span class="sxs-lookup"><span data-stu-id="d7bbd-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="d7bbd-122">A hitelesítésszolgáltató hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="d7bbd-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d7bbd-123">Hibaelhárítási házirend</span><span class="sxs-lookup"><span data-stu-id="d7bbd-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="d7bbd-124">Az Intune-eszközök megfelelőségét figyelve</span><span class="sxs-lookup"><span data-stu-id="d7bbd-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="d7bbd-125">Megjegyzés: Ezek a lépések csak az Azure Active Directory feltételes hozzáférés funkciójának hibaelhárításában lehetnek hasznosak.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="d7bbd-126">Az Exchange-házirend segítségével karanténba is lehet helyezni azt az eszközt, amely blokkolja az e-mail-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="d7bbd-127">Az Exchange-eszközök kezeléséről további információt [itt]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) talál.</span><span class="sxs-lookup"><span data-stu-id="d7bbd-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
