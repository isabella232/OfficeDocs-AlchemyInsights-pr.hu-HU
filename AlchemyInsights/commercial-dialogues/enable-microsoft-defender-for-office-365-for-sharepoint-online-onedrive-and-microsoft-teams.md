---
title: A Széf engedélyezése a SharePoint, a OneDrive és a Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894465"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>A Széf engedélyezése a SharePoint, a OneDrive és a Microsoft Teams

1. A globális rendszergazdai vagy biztonsági rendszergazdai hitelesítő adatokkal nyissa meg a Microsoft 365 Defender portált a -ban, majd a Házirendek & szabályok veszélyforrás-házirendek és Széf a Házirendek szakaszban válassza a <https://security.microsoft.com>  \>  \>  **Mellékletek** részt.

   Ha közvetlenül a Mellékletek **lapra Széf,** használja a következőt: <https://security.microsoft.com/safeattachmentv2> .

2. A **Mellékletek Széf** lapon kattintson a Globális **beállítások elemre.**
3. A megjelenő előjelen válassza A Microsoft Defender Office 365 for **SharePoint, OneDrive** és Microsoft Teams lehetőséget, majd válassza a Mentés **lehetőséget.**

    > [!TIP]
    >
    > Az alábbi lépésekkel fokozhatja a mellékletek Széf, SharePoint, OneDrive és Microsoft Teams:
    >
    > - Ha meg szeretné akadályozni, hogy a felhasználók kártékony fájlokat töltsenek le, használja a `$true` *DisallowInfectedFileDownload* paraméter értékét a **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** parancsmagon a SharePoint PowerShellben. További információért [lásd: A SharePoint PowerShell](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)használata a kártékony fájlok letöltésének megakadályozására.
    > - [Riasztási házirend létrehozása az észlelt fájlokhoz](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

További információt a Mellékletek a Széf, a Office 365 [a SharePoint,](https://go.microsoft.com/fwlink/?linkid=2092041)a OneDrive és a Microsoft Teams.
