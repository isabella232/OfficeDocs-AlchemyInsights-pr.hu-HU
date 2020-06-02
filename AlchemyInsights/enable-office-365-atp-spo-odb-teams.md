---
title: Az Office 365 ATP engedélyezése a SharePointhoz, a OneDrive-hoz és a Microsoft Teamshez
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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506920"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="0258f-102">Az Office 365 komplex veszélyforrások elleni védelmének engedélyezése a SharePoint Online, a OneDrive és a Microsoft Teams számára</span><span class="sxs-lookup"><span data-stu-id="0258f-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="0258f-103">Menjen https://protection.office.com és jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="0258f-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="0258f-104">Válassza **a Fenyegetéskezelési**  >  **házirend**  >  **biztonságos mellékleteit.**</span><span class="sxs-lookup"><span data-stu-id="0258f-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="0258f-105">Válassza **az ATP bekapcsolása a SharePoint, a OneDrive és a Microsoft Teams**esetén lehetőséget, majd kattintson a Mentés **gombra.**</span><span class="sxs-lookup"><span data-stu-id="0258f-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="0258f-106">(Ajánlott) Globális rendszergazdaként vagy SharePoint Online-rendszergazdaként futtassa a [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmalt úgy, hogy a **DisallowInfectedFileDownload** paraméter *értéke igaz.*</span><span class="sxs-lookup"><span data-stu-id="0258f-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="0258f-107">(Ajánlott) [Riasztások beállítása](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) az észlelt fájlokhoz.</span><span class="sxs-lookup"><span data-stu-id="0258f-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="0258f-108">Az ATP a SharePoint Online, a OneDrive vagy a Microsoft Teams minden egyes fájlját átvizsgál.</span><span class="sxs-lookup"><span data-stu-id="0258f-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="0258f-109">A fájlok ataszinkron módon, egy olyan folyamaton keresztül, amely megosztási és vendégtevékenységi eseményeket, valamint intelligens heurisztikát és fenyegetési jeleket használ a rosszindulatú fájlok azonosítására.</span><span class="sxs-lookup"><span data-stu-id="0258f-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="0258f-110">Lásd: [ATP for SharePoint, OneDrive és Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="0258f-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>