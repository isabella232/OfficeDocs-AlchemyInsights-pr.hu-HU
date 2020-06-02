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
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Az Office 365 komplex veszélyforrások elleni védelmének engedélyezése a SharePoint Online, a OneDrive és a Microsoft Teams számára

1. Menjen https://protection.office.com és jelentkezzen be.
2. Válassza **a Fenyegetéskezelési**  >  **házirend**  >  **biztonságos mellékleteit.**
3. Válassza **az ATP bekapcsolása a SharePoint, a OneDrive és a Microsoft Teams**esetén lehetőséget, majd kattintson a Mentés **gombra.**
4. (Ajánlott) Globális rendszergazdaként vagy SharePoint Online-rendszergazdaként futtassa a [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) parancsmalt úgy, hogy a **DisallowInfectedFileDownload** paraméter *értéke igaz.*
5. (Ajánlott) [Riasztások beállítása](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) az észlelt fájlokhoz.

> [!NOTE]
> Az ATP a SharePoint Online, a OneDrive vagy a Microsoft Teams minden egyes fájlját átvizsgál. A fájlok ataszinkron módon, egy olyan folyamaton keresztül, amely megosztási és vendégtevékenységi eseményeket, valamint intelligens heurisztikát és fenyegetési jeleket használ a rosszindulatú fájlok azonosítására. Lásd: [ATP for SharePoint, OneDrive és Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).