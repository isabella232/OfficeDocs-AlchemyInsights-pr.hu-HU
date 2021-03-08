---
title: E-mailek keresése és törlése a szervezetben
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524284"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="3df2e-102">E-mailek keresése és törlése a szervezetben</span><span class="sxs-lookup"><span data-stu-id="3df2e-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="3df2e-103">Hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="3df2e-103">Follow these steps:</span></span>

1. <span data-ttu-id="3df2e-104">Ha Ön nem globális rendszergazda, akkor az üzenetek kereséséhez fiókját fel kell venni az **Elektronikus** észleléskezelő szerepkörcsoportba vagy a Megfelelőségi keresés **kezelése szerepkörbe.**</span><span class="sxs-lookup"><span data-stu-id="3df2e-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="3df2e-105">Az üzenetek törléséhez csatlakoznia kell  a Szervezetkezelés szerepkörcsoporthoz vagy a Keresési és végleges **törlési szerepkörhöz.**</span><span class="sxs-lookup"><span data-stu-id="3df2e-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="3df2e-106">Az ezekre a szerepkörökre vonatkozó engedélyeket a Biztonsági & [megfelelőségi központban lehet hozzárendelni.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="3df2e-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="3df2e-107">[Hozzon létre tartalomkeresést](https://docs.microsoft.com/office365/securitycompliance/content-search) a törölni kívánt üzenet megkereshez.</span><span class="sxs-lookup"><span data-stu-id="3df2e-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="3df2e-108">[Csatlakozás a Biztonsági & Megfelelőségi központ PowerShell-parancshoz.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="3df2e-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="3df2e-109">Többtényezős hitelesítés használata esetén olvassa el a következő utasításokat: Csatlakozás a Biztonsági & Megfelelőségi központ [PowerShell-éhez többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="3df2e-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="3df2e-110">Törölje az üzenetet: futtassa `New-ComplianceSearchAction` a parancsmagot az üzenet törléséhez.</span><span class="sxs-lookup"><span data-stu-id="3df2e-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="3df2e-111">A törölt üzenetek a felhasználó Helyreállítható elemek mappájába kerülnek.</span><span class="sxs-lookup"><span data-stu-id="3df2e-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="3df2e-112">Az alábbi példaparancsot lásd: [3. lépés: Az üzenet törlése.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="3df2e-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
