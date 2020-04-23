---
title: Az Office 365 Komplex veszélyforrások elleni védelemmel (ATP) kapcsolatos problémák elhárítása
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766747"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="95d48-102">Az Office 365 ATP-vel kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="95d48-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="95d48-103">**Értesítés késések e-mail üzenet kézbesítés?**</span><span class="sxs-lookup"><span data-stu-id="95d48-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="95d48-104">Próbálja meg a dinamikus kézbesítési beállítást az ATP biztonságos mellékletek házirendjeihez.</span><span class="sxs-lookup"><span data-stu-id="95d48-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="95d48-105">Ezzel elkerülhető késés az e-mailek kézbesítése, miközben megvédi a címzetteket a rosszindulatú fájloktól.</span><span class="sxs-lookup"><span data-stu-id="95d48-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="95d48-106">**Hamis vagy hamis negatív okat szeretne jelenteni?**</span><span class="sxs-lookup"><span data-stu-id="95d48-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="95d48-107">Ezen a hivatkozáson keresztül elküldheti a fájlt elemzésre:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="95d48-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="95d48-108">**Tudta, hogy engedélyezheti az ATP Safe Links védelmét a szervezeten belüli személyek között küldött e-mailek számára?**</span><span class="sxs-lookup"><span data-stu-id="95d48-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="95d48-109">Hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="95d48-109">Follow these steps:</span></span>
    1. <span data-ttu-id="95d48-110">Nyissa https://protection.office.commeg a t, és jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="95d48-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="95d48-111">Nyissa meg a **Fenyegetéskezelési** > **házirend** > **biztonságos hivatkozásait.**</span><span class="sxs-lookup"><span data-stu-id="95d48-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="95d48-112">Az **adott címzettekre vonatkozó házirendek**csoportban szerkesztse (vagy adja hozzá) a házirendet.</span><span class="sxs-lookup"><span data-stu-id="95d48-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="95d48-113">Jelölje be **A szervezeten belül küldött üzenetekre mutató biztonságos hivatkozások alkalmazása**jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="95d48-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="95d48-114">Mentse a szabályzatot, és hagyjon körülbelül 30 percet arra, hogy a módosítások végighaladjanak az adatközponton.</span><span class="sxs-lookup"><span data-stu-id="95d48-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="95d48-115">Ha további segítségre van szüksége az ATP-vel kapcsolatban, olvassa el az [Office 365 Komplex veszélyforrások elleni védelem](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)ben.</span><span class="sxs-lookup"><span data-stu-id="95d48-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>