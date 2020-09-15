---
title: Az Office 365 ATP engedélyezése a SharePointhoz, a OneDrive és a Microsoft Teams alkalmazáshoz
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709909"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="b3af6-102">Az Office 365 Advanced Threat Protection engedélyezése a SharePoint Online, a OneDrive és a Microsoft Teams esetében</span><span class="sxs-lookup"><span data-stu-id="b3af6-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="b3af6-103">Ugrás https://protection.office.com és bejelentkezés.</span><span class="sxs-lookup"><span data-stu-id="b3af6-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="b3af6-104">Válassza a **veszélyforrások kezelése**a  >  **Policy**  >  **biztonságos mellékleteket**.</span><span class="sxs-lookup"><span data-stu-id="b3af6-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="b3af6-105">Jelölje be **az ATP bekapcsolása a sharepointhoz, a OneDrive és a Microsoft Teams**jelölőnégyzetet, és kattintson a **Mentés**gombra.</span><span class="sxs-lookup"><span data-stu-id="b3af6-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="b3af6-106">Ajánlott Globális rendszergazdaként vagy SharePoint Online-rendszergazdaként futtassa a [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmagot a **DisallowInfectedFileDownload** paraméter *true*értékre állításával.</span><span class="sxs-lookup"><span data-stu-id="b3af6-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="b3af6-107">Ajánlott Az észlelt fájlokra vonatkozó [értesítések beállítása](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) .</span><span class="sxs-lookup"><span data-stu-id="b3af6-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="b3af6-108">Az ATP a SharePoint Online, a OneDrive vagy a Microsoft Teams minden egyes fájljának beolvasását fogja tartalmazni.</span><span class="sxs-lookup"><span data-stu-id="b3af6-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="b3af6-109">A fájlok egy-egy megosztási és vendég-tevékenységi eseményeket használó folyamaton keresztül, valamint intelligens heurisztikus és veszélyforrás jelzésekkel beolvassák a kártékony fájlokat.</span><span class="sxs-lookup"><span data-stu-id="b3af6-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="b3af6-110">Lásd: [ATP for SharePoint, OneDrive és Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="b3af6-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>