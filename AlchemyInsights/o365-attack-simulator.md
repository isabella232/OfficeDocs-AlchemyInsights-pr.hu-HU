---
title: 2681 támadás Szimuláns hivatalban 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305334"
---
# <a name="attack-simulator-in-office-365"></a>Támadás Szimuláns hivatalban 365

- Van ön hiányzó támadás Szimuláns? Támadás szimulátor megkövetel **hivatal 365 haladó fenyeget védelem tervez 2 (ATP tervez 2)** vagy **Hivatal 365 vállalat E5**. Támadás Szimuláns van **nem** tartalmazott-ban Hivatal 365 haladó fenyeget védelem tervez 1 (ATP tervez 1), Hivatal 365 vállalat E3, vagy akármi Hivatal 365 teendő előfizetések.

- A szimulált támadások elindításához használt fióknak globális rendszergazdai vagy biztonsági rendszergazdai engedélyekre és többtényezős hitelesítésre van szüksége (MFA). A támadási követelményekkel kapcsolatos további tudnivalókért tanulmányozza ezt a [témakört](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Fontos dolgok tudni **brute force jelszó** támadás szimuláció:

  - Ha a célfiókhoz engedélyezve van az MFA, és a jelszó helyesen lett kitalálható, a fiók nem jelenik meg veszélybe (a második hitelesítési tényező nem lesz teljes).

  - A jelszófájl nem lehet nagyobb 10 MB-nál. Soronként egy jelszót használjon, és a lista utolsó jelszava után üres sort (kocsivissza) is használhat.

- Fontos tudnivalók a **lándzsával kapcsolatos adathalászó** szimulációkhoz:

  - Tervezéssel nem biztosíthat egyéni értéket az **adathalász bejelentkezési kiszolgáló URL-címének**.

  - Ha a címzett engedélyezi a [jelentésüzenet bővítmény](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) számára az üzenet adathalászattal történő jelentésének engedélyezését, akkor előfordulhat, hogy nem kap figyelmeztetést az üzenethez (mivel ez egy szimulált támadás).

- Jelentések: Miután befejeződött a szimulált támadás, a jelentés megtekintéséhez kattintson a **támadási adatok** gombra.

- Részére részletes oktatás és új jellegét meghatározza-ban támadás Szimuláns, lát [támadás Szimuláns hivatalban 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
