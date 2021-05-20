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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545728"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Attack in Microsoft 365

- Nem tudja, mi a támadás? A támadási rendszer **használatához a Microsoft Defender szükséges Office 365 2. vagy az** E5 Office 365 Nagyvállalati verzió **csomaghoz.** A Attack Defender **nem szerepel a** Microsoft Defender 1-es Office 365, Office 365 Nagyvállalati verzió E3 vagy bármilyen Üzleti Microsoft 365-alkalmazások előfizetésében.

- A szimulált támadások indításához használt fiókhoz globális rendszergazdai vagy biztonsági rendszergazdai engedélyek, valamint többtényezős hitelesítés (MFA) szükséges. A támadási rendszer követelményeiről további információt ebben [a témakörben található.](/microsoft-365/security/office-365-security/attack-simulator)

- Fontos tudni a **Találgatásos kényszerítéses** jelszó támadási szimulálásairól:

  - Ha a célfiókban engedélyezve van az MFA, és a jelszó helyesnek lett kitalálva, akkor a fiók nem jelenik meg feltörtként (a második hitelesítési tényező hiányos lesz).

  - A jelszófájl mérete nem lehet nagyobb 10 MB-nál. Sorbanként egy jelszót használjon, és a lista utolsó jelszava után használjon üres sort (kocsivissza).

- Fontos tudnivalók a **Phishing Phishing** csatolási szimulációkról:

  - Az adathalászó bejelentkezési kiszolgáló URL-címe úgy van megtervzve, hogy nem ad meg egyéni értéket az adathalászó bejelentkezési **kiszolgáló URL-címéhez.**

  - Ha egy címzett az [Enable the Report Message](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) (Jelentésüzenet engedélyezése) bővítményt használja az üzenet adathalászatként való bejelentéséhez, előfordulhat, hogy nem kap figyelmeztetést az üzenetről (mert ez szimulált támadás).

- Jelentések: Miután befejeződött a szimulált támadás, a Támadás részletei elemre kattintva láthatja a jelentést. 

- A támadási támadási szolgáltatás részletes útmutatóját és új funkcióit A támadási [Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)
