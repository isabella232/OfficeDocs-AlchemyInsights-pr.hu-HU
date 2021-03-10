---
title: Az Office 365- ös Microsoft Defender gyakori problémáinak elhárítása
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694031"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="00241-102">Az Office 365- ös Microsoft Defender gyakori problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="00241-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="00241-103">Íme néhány megoldás a Microsoft Defender office 365- ös verziójával kapcsolatos gyakori problémákra:</span><span class="sxs-lookup"><span data-stu-id="00241-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="00241-104">**Üzenetkéskés:** Ha olyan problémákat tapasztal, amelyek miatt késik az üzenetek  kézbesítése, a Biztonságos mellékletek házirend dinamikus kézbesítési beállításait kell használnia.</span><span class="sxs-lookup"><span data-stu-id="00241-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="00241-105">További információt a Dinamikus kézbesítés a Biztonságos mellékletek [házirendek között.](https://go.microsoft.com/fwlink/?linkid=2094106)</span><span class="sxs-lookup"><span data-stu-id="00241-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="00241-106">**Hamis pozitív vagy negatív eredmény jelentése:** Az üzenetet a Következő hivatkozással jelentse be a [Microsoftnak: Microsoft Defender válaszportál.](https://go.microsoft.com/fwlink/?linkid=2092835)</span><span class="sxs-lookup"><span data-stu-id="00241-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="00241-107">**Biztonságos hivatkozásvédelem engedélyezése:**</span><span class="sxs-lookup"><span data-stu-id="00241-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="00241-108">Jelentkezzen be az [Office 365 Biztonsági & Megfelelőségi központba.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="00241-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="00241-109">Ugrás a **veszélyforrás-kezelési**  >  **házirend biztonságos**  >  **hivatkozásaira.**</span><span class="sxs-lookup"><span data-stu-id="00241-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="00241-110">Az **adott címzettekre** vonatkozó házirendek alatt nyissa meg a konfigurált házirendet.</span><span class="sxs-lookup"><span data-stu-id="00241-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="00241-111">A **Beállítások csoportban** válassza a Biztonságos hivatkozások alkalmazása a szervezeten belül **küldött üzenetekre lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="00241-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
