---
title: A naptár ikon nem jelenik meg a Teams ügyfélprogramban
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819955"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="96cd9-102">A naptár ikon nem jelenik meg a Teams ügyfélprogramban</span><span class="sxs-lookup"><span data-stu-id="96cd9-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="96cd9-103">A Teams Naptár lapjához szükséges az Exchange-postaládához való hozzáférés a webes Exchange-szolgáltatásokon keresztül.</span><span class="sxs-lookup"><span data-stu-id="96cd9-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="96cd9-104">Az Exchange-postaláda lehet online vagy helyszíni.</span><span class="sxs-lookup"><span data-stu-id="96cd9-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="96cd9-105">Azon online felhasználók esetén, akiknek nem jelenik meg a Naptár lap, ellenőrizze, hogy [rendelkeznek-e licenccel az Exchange Online-postaládához, és a postaláda engedélyezett-e](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="96cd9-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="96cd9-106">Ha a felhasználó érvényes postaládával rendelkezik az Exchange Online-ban, ennek ellenére sem jelenik meg a Naptár lap, előfordulhat, hogy hálózati hibáról van szó.</span><span class="sxs-lookup"><span data-stu-id="96cd9-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="96cd9-107">A [Microsoft távkapcsolat-elemző eszközt](https://testconnectivity.microsoft.com/) használva futtassa a **Microsoft Exchange webszolgáltatások – kapcsolódási teszteket** az érintett felhasználó esetén.</span><span class="sxs-lookup"><span data-stu-id="96cd9-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="96cd9-108">Végül a [ Teams-appok appbeállítási szabályzatát](https://admin.teams.microsoft.com/policies/app-setup) ellenőrizve győződjön meg arról, hogy a Naptár app nem lett eltávolítva a felhasználóhoz (valószínűleg a **Globális (szervezeti szintű alapértelmezett)** alkalmazott szabályzatból.</span><span class="sxs-lookup"><span data-stu-id="96cd9-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="96cd9-109">Ha a felhasználók helyszínen tartózkodnak, meg kell erősítenie, hogy a hibrid konfiguráció állapota megfelelő.</span><span class="sxs-lookup"><span data-stu-id="96cd9-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="96cd9-110">A [Hibrid konfiguráció varázsló](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) használható a hibaelhárításhoz.</span><span class="sxs-lookup"><span data-stu-id="96cd9-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="96cd9-111">Felhívjuk a figyelmét, hogy a [Teamshez az Exchange 2016 CU3 vagy újabb verziója szükséges](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="96cd9-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
