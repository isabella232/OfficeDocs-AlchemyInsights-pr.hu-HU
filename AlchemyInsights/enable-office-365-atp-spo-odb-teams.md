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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>A Microsoft Defender engedélyezése Office 365 online SharePoint, OneDrive és Microsoft Teams

1. Jelentkezzen https://protection.office.com be.
2. Válassza **a Veszélyforrások elleni**  >  **Széf**  >  **mellékletek lehetőséget.**
3. Válassza **a Defender bekapcsolás a Office 365 a SharePoint,** a OneDrive és a Microsoft Teams lehetőséget, majd kattintson a Mentés **gombra.**
4. (Ajánlott) Globális rendszergazdaként vagy a SharePoint Online rendszergazdájaként futtassa a [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmagot úgy, hogy a **DisallowInfectedFileDownload** paraméter értéke *true*.
5. (Ajánlott) [Értesítések beállítása az](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) észlelt fájlokhoz.

> [!NOTE]
> A Microsoft Defender Office 365 nem vizsgálja meg az összes fájlt a SharePoint, a OneDrive és a Microsoft Teams. A fájlokat aszinkron módon, megosztási és vendégtevékenység-eseményeket használó folyamaton keresztül, intelligens heurisztikus és veszélyforrás-észleléssel azonosíthatja a kártékony fájlokat. Lásd: [Microsoft Defender Office 365 a SharePoint,](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)a OneDrive és a Microsoft Teams.