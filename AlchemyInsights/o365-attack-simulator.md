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
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895793"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Attack in Microsoft 365

- Nem tudja, mi a támadás? A támadási támadáshoz **a Microsoft Defender szükséges Office 365 2. vagy az** E5 Office 365 Nagyvállalati verzió **csomaghoz.** A Támadási lehetőséget **nem tartalmazza a** Microsoft Defender az 1-es Office 365, az E3 Office 365 Nagyvállalati verzió vagy bármilyen más Üzleti Microsoft 365-alkalmazások része.

- A szimulált támadások indításához használt fiókhoz globális rendszergazdai vagy biztonsági rendszergazdai engedélyek, valamint többtényezős hitelesítés (MFA) szükséges. A támadási rendszer követelményeiről további információt ebben [a témakörben található.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Fontos tudni a **Találgatásos kényszerítéses** jelszó támadási szimulálásairól:

  - Ha a célfiókban engedélyezve van az MFA, és a jelszó helyesnek lett kitalálva, a fiók nem jelenik meg feltörtként (a második hitelesítési tényező hiányos lesz).

  - A jelszófájl mérete nem lehet nagyobb 10 MB-nál. Sorbanként egy jelszót használjon, és a lista utolsó jelszava után használjon üres sort (kocsivissza).

- Fontos tudnivalók a **Phishing Phishing** csatolási szimulációkról:

  - Az adathalászó bejelentkezési kiszolgáló URL-címe úgy van megtervzve, hogy nem ad meg egyéni értéket az adathalászó bejelentkezési **kiszolgáló URL-címéhez.**

  - Ha egy címzett az [Enable the Report Message](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) (Jelentésüzenet engedélyezése) bővítményt használja az üzenet adathalászatként való bejelentéséhez, előfordulhat, hogy nem kap figyelmeztetést az üzenetről (mert ez szimulált támadás).

- Jelentések: Miután befejeződött a szimulált támadás, a Támadás részletei elemre kattintva láthatja a jelentést. 

- A támadási támadási és a támadási fogkomán megjelenő új funkciókról részletes útmutatást és funkciókat A [támadási](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)Microsoft 365.
