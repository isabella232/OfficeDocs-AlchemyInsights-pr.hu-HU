---
title: 2681-es támadási Microsoft 365
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
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325073"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Attack in Microsoft 365

- Nem tudja, mi a támadás? A támadási rendszer **használatához a Microsoft Defender szükséges Office 365 2. vagy az** E5 Office 365 Nagyvállalati verzió **csomaghoz.** A Támadási lehetőséget **nem tartalmazza a** Microsoft Defender az 1-es Office 365, az E3 Office 365 Nagyvállalati verzió- vagy Üzleti Microsoft 365-alkalmazások része.

- A szimulált támadások indításához használt fiókhoz globális rendszergazdai vagy biztonsági rendszergazdai engedélyek, valamint többtényezős hitelesítés (MFA) szükséges. A támadási rendszer követelményeiről további információt ebben [a témakörben található.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Fontos tudni a **Találgatásos kényszerítéses** jelszó támadási szimulálásairól:

  - Ha a célfiókban engedélyezve van az MFA, és a jelszó helyesnek lett kitalálva, a fiók nem jelenik meg feltörtként (a második hitelesítési tényező hiányos lesz).

  - A jelszófájl mérete nem lehet nagyobb 10 MB-nál. Sorbanként egy jelszót használjon, és a lista utolsó jelszava után használjon üres sort (kocsivissza).

- Fontos tudnivalók a **Phishing Phishing** csatolási szimulációkról:

  - Az adathalászó bejelentkezési kiszolgáló URL-címe úgy van megtervzve, hogy nem ad meg egyéni értéket az adathalászó bejelentkezési **kiszolgáló URL-címéhez.**

  - Ha egy címzett az [Enable the Report Message](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) (Jelentésüzenet engedélyezése) bővítményt használja az üzenet adathalászatként való bejelentéséhez, előfordulhat, hogy nem kap figyelmeztetést az üzenetről (mert ez szimulált támadás).

- Jelentések: Miután befejeződött a szimulált támadás, a Támadás részletei elemre kattintva láthatja a jelentést. 

- A támadási és új funkcióiról részletes útmutatást és új funkciókat A támadási [Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
