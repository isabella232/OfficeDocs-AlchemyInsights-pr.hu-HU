---
title: Intune feltételes hozzáférés figyelése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427920"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="6c367-102">Intune feltételes hozzáférés figyelése</span><span class="sxs-lookup"><span data-stu-id="6c367-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="6c367-103">A feltételes hozzáféréssel megcélzott felhasználók értesítést kapnak e-mailben, ha nem teljesítik a szervezet hozzáférési követelményeit.</span><span class="sxs-lookup"><span data-stu-id="6c367-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6c367-104">A probléma megoldásához az alábbi megoldásokat javasoljuk:</span><span class="sxs-lookup"><span data-stu-id="6c367-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="6c367-105">Ha az eszköz regisztrálva van, javasolja a felhasználónak, hogy a Céges portál appban ellenőrizze, hogy megjelenik-e a céges portálon.</span><span class="sxs-lookup"><span data-stu-id="6c367-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6c367-106">Ha nem, a felhasználónak regisztrálnia kell az eszközt.</span><span class="sxs-lookup"><span data-stu-id="6c367-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="6c367-107">Az Azure Portalon az  >  **Intune-eszközök megfelelőségét.**</span><span class="sxs-lookup"><span data-stu-id="6c367-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="6c367-108">Ha meg kell tekintenie az eszközre vonatkozó megfelelőségi jelentést, és ellenőriznie kell, hogy a felhasználó eszköze kompatibilisként van-e megjelölve, a **Figyelés** csoportban kattintson az **Eszköz megfelelősége elemre.**</span><span class="sxs-lookup"><span data-stu-id="6c367-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="6c367-109">Az Azure Portalon az  >  **Intune-eszközök megfelelőségét.**</span><span class="sxs-lookup"><span data-stu-id="6c367-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="6c367-110">A **Kezelés alatt kattintson** a **Házirendek elemre.**</span><span class="sxs-lookup"><span data-stu-id="6c367-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="6c367-111">A megfelelőségi szabályzatok listájában ellenőrizze, hogy van-e profil hozzárendelve a felhasználó eszközéhez.</span><span class="sxs-lookup"><span data-stu-id="6c367-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6c367-112">Ha nincs hozzárendelve profil, akkor az Intune nem fogja tudni megerősíteni az eszköz megfelelőségi állapotát.</span><span class="sxs-lookup"><span data-stu-id="6c367-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="6c367-113">Szerkessze a felhasználó feltételes hozzáférési hozzárendelését.</span><span class="sxs-lookup"><span data-stu-id="6c367-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="6c367-114">Az Azure Portalon lépjen az **Intune** feltételes hozzáférési szabályzatához, válasszon ki egy házirendet  >    >  a listából, és kattintson a Felhasználók és csoportok **elemre.**</span><span class="sxs-lookup"><span data-stu-id="6c367-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="6c367-115">Ha meg szeretne adni egy házirendet valakinél, vegye fel a házirendet a Felvétel **listára.**</span><span class="sxs-lookup"><span data-stu-id="6c367-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="6c367-116">Ha ki szeretne hagyni egy személyt a házirendből, vegye fel őket a Kizárás **listára.**</span><span class="sxs-lookup"><span data-stu-id="6c367-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="6c367-117">**Hasznos hivatkozások:**</span><span class="sxs-lookup"><span data-stu-id="6c367-117">**Helpful links:**</span></span>

- [<span data-ttu-id="6c367-118">Eszköz-megfelelőség áttekintése</span><span class="sxs-lookup"><span data-stu-id="6c367-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="6c367-119">A hitelesítésszolgáltató hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="6c367-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="6c367-120">Hibaelhárítási házirend</span><span class="sxs-lookup"><span data-stu-id="6c367-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="6c367-121">Az Intune-eszközök megfelelőségét figyelve</span><span class="sxs-lookup"><span data-stu-id="6c367-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="6c367-122">Ezek a lépések csak az Azure Active Directory feltételes hozzáférés funkciójának hibaelhárításában lehetnek hasznosak.</span><span class="sxs-lookup"><span data-stu-id="6c367-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="6c367-123">Az Exchange-házirend segítségével karanténba is lehet helyezni azt az eszközt, amely blokkolja az e-mail-hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="6c367-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="6c367-124">Az Exchange-eszközök kezeléséről itt [**talál további információt.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="6c367-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
