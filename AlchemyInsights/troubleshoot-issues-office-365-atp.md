---
title: Az Office 365 Advanced Threat Protection (ATP) hibáinak elhárítása
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758067"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="5d7db-102">Az Office 365 ATP hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="5d7db-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="5d7db-103">**Észleli az e-mailek kézbesítésének késleltetését**?</span><span class="sxs-lookup"><span data-stu-id="5d7db-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="5d7db-104">Használja a dinamikus kézbesítési lehetőséget az ATP-Safe mellékletek házirendjében.</span><span class="sxs-lookup"><span data-stu-id="5d7db-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="5d7db-105">Így elkerülhető az e-mailek kézbesítésének késleltetése, miközben megvédi a címzetteket a kártékony fájlokból.</span><span class="sxs-lookup"><span data-stu-id="5d7db-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="5d7db-106">**Hamis pozitív vagy hamis negatívokat szeretne jelenteni**?</span><span class="sxs-lookup"><span data-stu-id="5d7db-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="5d7db-107">Ezzel a hivatkozással elküldheti a fájlt elemzés céljából: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="5d7db-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="5d7db-108">**Tudta, hogy engedélyezheti az ATP Safe Links Protectiont a szervezete tagjai között küldött e-mailek védelméhez**?</span><span class="sxs-lookup"><span data-stu-id="5d7db-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="5d7db-109">Hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="5d7db-109">Follow these steps:</span></span>
    1. <span data-ttu-id="5d7db-110">Kattintson a gombra https://protection.office.com , és a Bejelentkezés gombra.</span><span class="sxs-lookup"><span data-stu-id="5d7db-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="5d7db-111">Nyissa meg a **veszélyforrások kezelése**  >  **házirendben**lévő  >  **biztonságos hivatkozásokat**.</span><span class="sxs-lookup"><span data-stu-id="5d7db-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="5d7db-112">A **meghatározott címzettekre vonatkozó házirendek**csoportban szerkessze (vagy vegye fel) a házirendet.</span><span class="sxs-lookup"><span data-stu-id="5d7db-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="5d7db-113">Válassza **a biztonságos hivatkozások alkalmazása a szervezeten belül küldött üzenetekre**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="5d7db-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="5d7db-114">Mentse a házirendet, és a változtatások körülbelül 30 perc alatt dolgozhassanak az adatközponton keresztül.</span><span class="sxs-lookup"><span data-stu-id="5d7db-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="5d7db-115">Ha további segítségre van szüksége az ATP szolgáltatáshoz, olvassa el az [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)című témakört.</span><span class="sxs-lookup"><span data-stu-id="5d7db-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>