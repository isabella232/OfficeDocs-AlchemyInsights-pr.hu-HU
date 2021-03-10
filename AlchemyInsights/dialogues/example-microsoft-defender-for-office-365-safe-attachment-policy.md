---
title: 'Példa: Microsoft Defender az Office 365 biztonságos mellékletre vonatkozó házirendje'
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693827"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="d7963-102">Példa: Microsoft Defender az Office 365 biztonságos mellékletre vonatkozó házirendje</span><span class="sxs-lookup"><span data-stu-id="d7963-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="d7963-103">Ezek a beállítások engedélyezik a *"Nincs* késés" házirendet, amely azonnal kézbesíti az üzeneteket, majd a beolvasás után újra csatolja a mellékleteket:</span><span class="sxs-lookup"><span data-stu-id="d7963-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="d7963-104">**Név:** Nincs késés</span><span class="sxs-lookup"><span data-stu-id="d7963-104">**Name**: No delays</span></span>
- <span data-ttu-id="d7963-105">**Leírás:** Azonnal kézbesíti az üzeneteket, és a beolvasás után újra beolvassa a mellékleteket.</span><span class="sxs-lookup"><span data-stu-id="d7963-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="d7963-106">**Válasz:** Válassza a **Dinamikus kézbesítés lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d7963-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="d7963-107">További információt a Dinamikus kézbesítés a Biztonságos mellékletek [házirendek között.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="d7963-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="d7963-108">**Mellékletek** átirányítása szakasz: Válassza az Átirányítás engedélyezése **lehetőséget,** majd adja meg a Microsoft 365 globális rendszergazdájának, biztonsági rendszergazdájának vagy biztonsági elemzőnek az e-mail-címét, aki vizsgálja a kártékony mellékleteket.</span><span class="sxs-lookup"><span data-stu-id="d7963-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="d7963-109">**Alkalmazott szakasz:** Jelölje ki a **címzett tartományát,** majd jelölje ki a tartományát.</span><span class="sxs-lookup"><span data-stu-id="d7963-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="d7963-110">Válassza **a Hozzáadás** gombot, majd az OK **gombot.**</span><span class="sxs-lookup"><span data-stu-id="d7963-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="d7963-111">Ha végzett, válassza a **Mentés gombot.**</span><span class="sxs-lookup"><span data-stu-id="d7963-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="d7963-112">További információt a Biztonságos mellékletek az [Office 365-hez való Microsoft Defenderben.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="d7963-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
