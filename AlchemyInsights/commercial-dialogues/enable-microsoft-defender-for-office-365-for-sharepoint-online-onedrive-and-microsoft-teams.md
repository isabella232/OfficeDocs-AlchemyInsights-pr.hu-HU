---
title: A Microsoft Defender engedélyezése az Office 365-hez a SharePoint Online-hoz, a OneDrive-hoz és a Microsoft Teamshez
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745304"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="9c1db-102">A Microsoft Defender engedélyezése az Office 365-hez a SharePoint Online-hoz, a OneDrive-hoz és a Microsoft Teamshez</span><span class="sxs-lookup"><span data-stu-id="9c1db-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="9c1db-103">Jelentkezzen be az Office 365 Biztonsági és megfelelőségi központba globális rendszergazdai vagy biztonsági [rendszergazdai hitelesítő adataival.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="9c1db-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="9c1db-104">A **bal oldali** ablaktáblában válassza a Veszélyforrások kezelése, majd a **Házirend** biztonságos  >  [mellékletek lehetőséget.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="9c1db-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="9c1db-105">Válassza **A Microsoft Defender bekapcsolás az Office 365-hez a SharePointhoz, a OneDrive-hoz** és a Microsoft Teamshez lehetőséget, majd válassza a Mentés **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="9c1db-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="9c1db-106">Globális rendszergazdaként vagy SharePoint Online-rendszergazdaként futtassa a következő PowerShell-parancsmagot a **DisallowInfectedFileDownload** paraméter igaz *értékével:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="9c1db-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="9c1db-107">Értesítések beállítása az észlelt fájlokhoz</span><span class="sxs-lookup"><span data-stu-id="9c1db-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="9c1db-108">További információ: [Microsoft Defender a SharePointhoz,](https://go.microsoft.com/fwlink/?linkid=2092041)a OneDrive-hoz és a Microsoft Teamshez.</span><span class="sxs-lookup"><span data-stu-id="9c1db-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
