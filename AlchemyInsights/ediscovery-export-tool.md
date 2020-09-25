---
title: eDiscovery exportálási eszköze
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277924"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nem lehet telepíteni vagy futtatni az eDiscovery exportálási eszközét?

Ha nem tudja telepíteni vagy futtatni az eDiscovery exportálási eszközét a keresési eredmények letöltéséhez, ellenőrizze az alábbi dolgokat:
  
- A használt számítógép megfelel az alábbi előfeltételeknek:

  - a Windows 7 és a későbbi verziók 32-vagy 64-bites verziója

  - Microsoft .NET Framework 4.7

  - Támogatott böngésző:

  - Microsoft Edge

    Vagy

  - Internet Explorer 10 vagy újabb verziók

    Más böngészők, mint például a Google Chrome és a Mozilla Firefox, nem támogatottak.

- Szervezete elérheti a végpontot az Azure-ban, amely ** \* . blob.Core.Windows.net** (a helyettesítő karakter az exportálási feladat egyedi azonosítóját jelenti).

- Az exportálási szerepkört hozzárendelte a Microsoft 365 biztonsági &amp; megfelelőségi központban. Alapértelmezés szerint ez a szerepkör csak az eDiscovery-kezelő szerepkörcsoport szerepkör-csoportjához van társítva. Lásd: [eDiscovery-engedélyek hozzárendelése](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

További információt a tartalmi találatok [exportálása](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)című témakörben találhat.

Ha több, mint 100K postaládát exportál, a következő PowerShell-lel kell használnia az Exportálás eredményének letöltéséhez:  [eredmények exportálása több mint 100k postaládából](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).