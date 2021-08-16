---
title: A Microsoft Defender engedélyezése Office 365 online SharePoint, OneDrive és Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058868"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>A Microsoft Defender engedélyezése Office 365 online SharePoint, OneDrive és Microsoft Teams

1. Jelentkezzen be az Office 365 Biztonsági és megfelelőségi központba globális rendszergazdai vagy biztonsági rendszergazdai hitelesítő [adataival.](https://protection.office.com/)
2. A **bal oldali** ablaktáblában válassza a Veszélyforrások kezelése gombra, majd a Házirendkezelés  >  [Széf gombra.](https://protection.office.com/safeattachment)
3. Válassza **A Microsoft Defender bekapcsolás a Office 365, SharePoint, OneDrive és Microsoft Teams lehetőséget,** majd válassza a Mentés **lehetőséget.**
    > [!TIP]
    >
    > - Globális vagy SharePoint Online-rendszergazdaként futtassa az alábbi PowerShell-parancsmagot a **DisallowInfectedFileDownload** paraméter igaz *értékével:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Értesítések beállítása az észlelt fájlokhoz](https://go.microsoft.com/fwlink/?linkid=2092110)

További információ: [Microsoft Defender Office 365 a SharePoint, a OneDrive és](https://go.microsoft.com/fwlink/?linkid=2092041)a Microsoft Teams.
