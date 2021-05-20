---
title: A Office 365, a SharePoint, a OneDrive és a Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543930"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ab929-102">A Microsoft Defender engedélyezése Office 365 online SharePoint, OneDrive és Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ab929-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ab929-103">Jelentkezzen https://protection.office.com be.</span><span class="sxs-lookup"><span data-stu-id="ab929-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ab929-104">Válassza **a Veszélyforrások elleni**  >  **Széf**  >  **mellékletek lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ab929-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="ab929-105">Válassza **a Defender bekapcsolás a Office 365 a SharePoint,** a OneDrive és a Microsoft Teams lehetőséget, majd kattintson a Mentés **gombra.**</span><span class="sxs-lookup"><span data-stu-id="ab929-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="ab929-106">(Ajánlott) Globális rendszergazdaként vagy a SharePoint Online rendszergazdájaként futtassa a [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmagot úgy, hogy a **DisallowInfectedFileDownload** paraméter értéke *true*.</span><span class="sxs-lookup"><span data-stu-id="ab929-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="ab929-107">(Ajánlott) [Értesítések beállítása az](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) észlelt fájlokhoz.</span><span class="sxs-lookup"><span data-stu-id="ab929-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ab929-108">A Microsoft Defender Office 365 nem vizsgálja meg az összes fájlt a SharePoint, a OneDrive és a Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ab929-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ab929-109">A fájlokat aszinkron módon, megosztási és vendégtevékenység-eseményeket használó folyamaton keresztül, intelligens heurisztikus és veszélyforrás-észleléssel azonosíthatja a kártékony fájlokat.</span><span class="sxs-lookup"><span data-stu-id="ab929-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ab929-110">Lásd: [Microsoft Defender Office 365 a SharePoint,](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)a OneDrive és a Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ab929-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>