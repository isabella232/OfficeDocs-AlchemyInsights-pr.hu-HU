---
title: Ígérethez rendelkezésre álló mennyiség, a SharePoint, a OneDrive és a Microsoft csapatok
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765124"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="c4ca2-102">Ígérethez rendelkezésre álló mennyiség, a SharePoint, a OneDrive és a Microsoft csapatok</span><span class="sxs-lookup"><span data-stu-id="c4ca2-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="c4ca2-103">Kövesse az alábbi lépéseket ahhoz, hogy speciális fenyegetés védelme:</span><span class="sxs-lookup"><span data-stu-id="c4ca2-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="c4ca2-104">Ugrás a [https://protection.office.com](https://protection.office.com) és a globális rendszergazdai vagy biztonsági rendszergazdai fiókkal jelentkezzen.</span><span class="sxs-lookup"><span data-stu-id="c4ca2-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="c4ca2-105">A **fenyegetés kezelés**alatt a bal oldali ablaktáblában, válassza a **házirend** \> **Biztonságos mellékletek**.</span><span class="sxs-lookup"><span data-stu-id="c4ca2-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="c4ca2-106">Válassza az **Ígérethez rendelkezésre álló mennyiség, a SharePoint, a OneDrive, és a Microsoft csapatok**.</span><span class="sxs-lookup"><span data-stu-id="c4ca2-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="c4ca2-107">A [riasztási tevékenység házirend létrehozása](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) , hogy értesítést kapjon, ha azt észleli, hogy rosszindulatú fájlokat.</span><span class="sxs-lookup"><span data-stu-id="c4ca2-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="c4ca2-108">Részletes utasításokért lásd: Ez a [témakör](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c4ca2-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="c4ca2-109">**Megjegyzés**: úgy tervezték, ATP nem ellenőrzi minden SharePoint Online, a OneDrive egyetlen fájlban üzleti, vagy a Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c4ca2-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="c4ca2-110">Fájlok aszinkron beolvasott megosztási tevékenység, tevékenység Vendég használó folyamatok és fenyegető jeleket rosszindulatú fájlok azonosítása.</span><span class="sxs-lookup"><span data-stu-id="c4ca2-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="c4ca2-111">További tudnivalókért tanulmányozza a [témakör](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c4ca2-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
