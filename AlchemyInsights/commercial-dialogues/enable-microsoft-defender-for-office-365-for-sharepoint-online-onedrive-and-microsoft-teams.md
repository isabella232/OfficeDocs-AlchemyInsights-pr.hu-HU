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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>A Microsoft Defender engedélyezése az Office 365-hez a SharePoint Online-hoz, a OneDrive-hoz és a Microsoft Teamshez

1. Jelentkezzen be az Office 365 Biztonsági és megfelelőségi központba globális rendszergazdai vagy biztonsági [rendszergazdai hitelesítő adataival.](https://protection.office.com/)
2. A **bal oldali** ablaktáblában válassza a Veszélyforrások kezelése, majd a **Házirend** biztonságos  >  [mellékletek lehetőséget.](https://protection.office.com/safeattachment)
3. Válassza **A Microsoft Defender bekapcsolás az Office 365-hez a SharePointhoz, a OneDrive-hoz** és a Microsoft Teamshez lehetőséget, majd válassza a Mentés **lehetőséget.**
    > [!TIP]
    >
    > - Globális rendszergazdaként vagy SharePoint Online-rendszergazdaként futtassa a következő PowerShell-parancsmagot a **DisallowInfectedFileDownload** paraméter igaz *értékével:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Értesítések beállítása az észlelt fájlokhoz](https://go.microsoft.com/fwlink/?linkid=2092110)

További információ: [Microsoft Defender a SharePointhoz,](https://go.microsoft.com/fwlink/?linkid=2092041)a OneDrive-hoz és a Microsoft Teamshez.
