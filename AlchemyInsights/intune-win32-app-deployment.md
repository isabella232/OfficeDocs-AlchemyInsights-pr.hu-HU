---
title: Intune win32 app-telepítő
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461870"
---
# <a name="intune-win32-app-deployment"></a>Intune win32 app-telepítő

A Microsoft Intune lehetővé teszi a Win32-alkalmazásokat, például az MSI-t és az Office-t. Az EXE-fájlt Windows 10-es eszközökre kell telepíteni. A használt központi telepítési mechanizmushoz az Intune felügyeleti bővítmény (IME) szükséges a céleszköz megadásához. Az ÍRÁSJEGYBEVIVŐt automatikusan telepíti a rendszer a PowerShell-parancsfájlok vagy a Win32-alkalmazások felhasználóhoz vagy eszközhöz való telepítésének eredményeképpen.

Vannak olyan előfeltételek is, amelyeknek teljesíteniük kell a Win32 alkalmazások központi telepítéséhez, amelyek a következők:

- Támogatott platformok: a Windows 10 1607-es vagy újabb verziója (nagyvállalati, Pro-és oktatási verzió).
- Támogatott architektúra: x86 és x64.
- Eszközkezelés: a AAD csatlakozott és automatikusan regisztrált (többek között a hibrid tartomány csatlakozott és a csoportházirend automatikus igénylése).
- Alkalmazásspecifikus csomag formátuma:. a [Microsoft Win32 Content PREP Tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)által készített **intunewin** -fájl
- Korlátozások
    - Maximális méret: 8GB.
    - Nem támogatott architektúra: karok.

A fenti lépésekkel kapcsolatos további tudnivalókért olvassa el a[Win32-alkalmazás hozzáadása, hozzárendelése és figyelése a Microsoft Intune-ban](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)című témakört.

A Windows és a Win32 alkalmazások hibaelhárítási alkalmazásainak ismertetése a következő dokumentumokban olvasható.

- [Az alkalmazások telepítésével kapcsolatos hibák elhárítása](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32-alkalmazások – hibaelhárítás](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)