---
title: 2681-os támadás szimulátor a Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801553"
---
# <a name="attack-simulator-in-microsoft-365"></a>Támadási szimulátor a Microsoft 365

- Hiányzik a támadási szimulátor? A támadás-szimulátor használatához **a Microsoft Defender for office 365 Plan 2 (ATP-csomag 2) vagy az** **Office 365 nagyvállalati E5** csomag szükséges. A támadási szimulátor **nem** része a Microsoft Defender for Office 365 (ATP-csomag), az Office 365 Enterprise E3 csomagnak vagy bármely Microsoft 365-alkalmazás vállalati verziós előfizetésnek.

- A szimulált támadások elindításához használt fiók globális rendszergazdai vagy biztonsági rendszergazdai engedélyekkel és többtényezős hitelesítéssel (MFA) szükséges. A támadási szimulátor követelményeiről a következő [témakörben](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)olvashat bővebben.

- Fontos tudnivalók a **brute force jelszó** -támadási szimulációról:

  - Ha a célcella engedélyezve van, és a jelszó helyes volt, a fiók nem fog megjelenni a kiegyezésként (a második hitelesítési tényező hiányos lesz).

  - A jelszó-fájl nem lehet nagyobb 10 MB-nál. Használjon soronként egy jelszót, és vegyen fel egy üres vonalat (kocsivissza) a lista utolsó jelszava után.

- Fontos tudni, hogy a **célzott adathalászat** -szimulációk:

  - A terv szerint nem tud egyéni értéket biztosítani az **adathalászati bejelentkezési kiszolgáló URL-címéhez** .

  - Ha a címzettek [engedélyezik a jelentéskészítő üzenetben](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) az üzenet adathalászatként való jelentését, előfordulhat, hogy nem kap értesítést az üzenetről (mert szimulált támadás).

- Jelentések: a szimulált támadás befejeződése után a **támadás részletei** hivatkozásra kattintva megtekintheti a jelentést.

- A támadási szimulátorban a következő témakörben talál részletes útmutatást és új funkciókat: a [támadás szimulátor a Microsoft 365-ban](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
