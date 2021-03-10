---
title: A Microsoft Defender engedélyezése a SharePoint Online-hoz, a OneDrive-hoz és a Microsoft Teamshez elérhető Office 365-hez
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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694043"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>A Microsoft Defender engedélyezése a SharePoint Online-hoz, a OneDrive-hoz és a Microsoft Teamshez elérhető Office 365-hez

1. Jelentkezzen be az Office 365 Biztonsági és megfelelőségi központba globális rendszergazdai vagy biztonsági [rendszergazdai hitelesítő adataival.](https://protection.office.com/)
2. A **bal oldali** ablaktáblában válassza a Veszélyforrások kezelése lehetőséget, majd válassza a **Házirend** biztonságos  >  [mellékletek lehetőséget.](https://protection.office.com/safeattachment)
3. Válassza **a Microsoft Defender bekapcsolás az Office 365-hez a SharePointhoz, a OneDrive-hoz** és a Microsoft Teamshez, majd a Mentés **lehetőséget.**
    > [!TIP]
    >
    > - Globális rendszergazdaként vagy SharePoint Online-rendszergazdaként futtassa az alábbi PowerShell-parancsmagot úgy, hogy a **DisallowInfectedFileDownload** paraméter értéke *igaz:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Értesítések beállítása az észlelt fájlokhoz](https://go.microsoft.com/fwlink/?linkid=2092110)

További információt a [Microsoft Defender for Office 365 for SharePoint, OneDrive](https://go.microsoft.com/fwlink/?linkid=2092041)és Microsoft Teams webhelyen található.
