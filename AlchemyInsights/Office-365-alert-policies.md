---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 7bb5ec0efb7e29dc6a133d62491c7674c5a851a4fa422c647035aeaa0dbcd8d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918361"
---
# <a name="alert-policies"></a>Riasztási házirendek

Az Microsoft 365 biztonsági & megfelelőségi központban [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) alapértelmezett riasztási házirendek gára vannak beállítva, amelyek riasztásokat indítnak az Office 365 Nagyvállalati verzió vagy Office 365 Us Government E1/G1, E3/G3 vagy E5/G5 előfizetéssel. Ezért előfordulhat, hogy a rendszergazdák értesítést kapnak az e-mailben, amelyet a Office365Alerts@microsoft.com küld egy tárgysorsal, például "Kis súlyosságú riasztás: a riasztási házirend *neve".* A riasztási értesítéseket a rendszer akkor küldi el, ha gyakori tevékenységekre, például a felhasználókra vonatkozó riasztások aktiválódnak:

- Levelezési szabályokat hozhat létre, amelyek továbbítják az e-maileket.
- Rendelje hozzá a postaládához az engedélyeket.
- Nagyszámú fájlt oszthat meg vagy törölhet SharePoint fájlmegosztáskor.
- Elektronikus adatfelkereséseket hozhat létre, és exportálhatja a keresési eredményeket.

Értesítés áttekintése és az arra vonatkozó jogi eljárás:

1. Jelentkezzen be [a Biztonsági & megfelelőségi központba.](https://protection.office.com)
2. Kattintson **az Értesítések megtekintése**  >  **riasztások elemre.**
3. Az értesítésre kattintva megjeleníthet egy figyelmeztető lapot, amely információkat tartalmaz az értesítésről.

Az értesítéseken műveletet is el lehet távolítani, például el kell [távolítania egy gyanús beérkezett üzenetekre vonatkozó szabályt.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Vagy egyszerűen zárja be a  riasztást az értesítési lapon a Feloldás gombra kattintva.

A riasztási házirendek konfigurálásával és kezelésével kapcsolatos további tudnivalók ebben [a cikkben olvashatók.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Fontos:** A Microsoft e-mail-értesítésekkel kapcsolatos értesítései soha nem kérik az alábbiakra:

- Jelszó megadása
- A fiók biztonsági részleteinek ellenőrzése
- Saját hitelesítés újra

Ha ilyen e-mailt kap, azt a Microsoft nem küldte el, és adathalász üzenetnek minősül. Ha ez történik, [jelentse a Microsoftnak.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)