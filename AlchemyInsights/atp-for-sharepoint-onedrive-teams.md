---
title: ATP a SharePointhoz, a OneDrive-hoz és a Microsoft Teamshez
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508414"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="1d66c-102">ATP a SharePointhoz, a OneDrive-hoz és a Microsoft Teamshez</span><span class="sxs-lookup"><span data-stu-id="1d66c-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="1d66c-103">A komplex veszélyforrások elleni védelem engedélyezéséhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="1d66c-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="1d66c-104">Lépjen a [https://protection.office.com](https://protection.office.com) globális rendszergazdai vagy biztonsági rendszergazdai fiókkal, és jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="1d66c-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="1d66c-105">A **fenyegetéskezelés**csoport bal oldali **Policy** navigációs ablakában válassza a \> **Házirend biztonságos mellékletei**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1d66c-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="1d66c-106">Válassza **az ATP bekapcsolása lehetőséget a SharePoint, a OneDrive és a Microsoft Teams számára.**</span><span class="sxs-lookup"><span data-stu-id="1d66c-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="1d66c-107">[Hozzon létre egy tevékenységriasztási szabályzatot,](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) amely értesítéseket kap a kártékony fájlok észlelésekor.</span><span class="sxs-lookup"><span data-stu-id="1d66c-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="1d66c-108">A teljes körű útmutatást lásd ebben a [témakörben](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="1d66c-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="1d66c-109">**Megjegyzés:** Az ATP nem vizsgál be minden egyes fájlt a SharePoint Online-ban, a OneDrive Vállalati verzióban vagy a Microsoft Teamsben.</span><span class="sxs-lookup"><span data-stu-id="1d66c-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="1d66c-110">A fájlokat aszinkron módon egy olyan folyamat ellenőrzi, amely megosztási tevékenységet, vendégtevékenységet és fenyegetésjelzéseket használ a rosszindulatú fájlok azonosítására.</span><span class="sxs-lookup"><span data-stu-id="1d66c-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="1d66c-111">További információt ebben a [témakörben talál.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="1d66c-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
