---
title: ATP a SharePointhoz, a OneDrive-hoz és a Microsoft Teams-hoz
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715563"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="0073e-102">ATP a SharePointhoz, a OneDrive-hoz és a Microsoft Teams-hoz</span><span class="sxs-lookup"><span data-stu-id="0073e-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="0073e-103">A speciális veszélyforrások elleni védelem engedélyezéséhez kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="0073e-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="0073e-104">Lépjen [https://protection.office.com](https://protection.office.com) egy globális rendszergazdai vagy biztonsági rendszergazdai fiókjával, és lépjen be.</span><span class="sxs-lookup"><span data-stu-id="0073e-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="0073e-105">A bal oldali navigációs ablakban a **fenyegetések kezelése**csoportban válassza a **házirend** - \> **megbízható mellékletek**elemet.</span><span class="sxs-lookup"><span data-stu-id="0073e-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="0073e-106">Válassza **az ATP bekapcsolása a SharePointban, a OneDrive és a Microsoft Teams szolgáltatásban**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0073e-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="0073e-107">[Tevékenység-figyelmeztetési házirend létrehozása](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) a kártékony fájlok észlelése esetén.</span><span class="sxs-lookup"><span data-stu-id="0073e-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="0073e-108">A teljes útmutatásért olvassa el ezt a [témakört](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="0073e-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="0073e-109">**Megjegyzés**: a terv szerint az ATP nem vizsgálja meg a SharePoint Online, a OneDrive vállalati verzió vagy a Microsoft Teams minden egyes fájlját.</span><span class="sxs-lookup"><span data-stu-id="0073e-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="0073e-110">A fájlokat a program aszinkron módon vizsgálja át egy olyan eljárással, amely a megosztási tevékenységet, a vendégeket és a fenyegetéseket használja a kártékony fájlok felismeréséhez.</span><span class="sxs-lookup"><span data-stu-id="0073e-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="0073e-111">További információt ebben a [témakörben](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)talál.</span><span class="sxs-lookup"><span data-stu-id="0073e-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
