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
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312689"
---
# <a name="alert-policies"></a>Riasztási házirendek

Microsoft 365 alapértelmezett riasztási házirendeket tartalmaz, amelyek riasztásokat indítnak a Microsoft 365 Nagyvállalati verzió vagy Microsoft 365 Kormányzati E1/G1, E3/G3 vagy E5/G5 előfizetéssel. [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) Ezért előfordulhat, hogy a rendszergazdák értesítést kapnak az e-mailben, amelyet a Office365Alerts@microsoft.com küld egy tárgysorsal, például "Kis súlyosságú riasztás: a riasztási házirend *neve".* A riasztási értesítéseket a rendszer akkor küldi el, ha gyakori tevékenységekre, például a felhasználókra vonatkozó riasztások aktiválódnak:

- Levelezési szabályokat hozhat létre, amelyek továbbítják az e-maileket.
- Rendelje hozzá a postaládához az engedélyeket.
- Nagyszámú fájlt oszthat meg vagy törölhet SharePoint fájlmegosztáskor.
- Elektronikus adatfelkereséseket hozhat létre, és exportálhatja a keresési eredményeket.

Értesítés áttekintése és az arra vonatkozó jogi eljárás:

1. Tegye a következők valamelyikét:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> riasztások **ot.** Vagy közvetlenül a Riasztások **lapra** való ugráshoz használja a <https://compliance.microsoft.com/compliancealerts> következőt: .
   - A Microsoft 365 Defender portálon a <https://security.microsoft.com> következőt: **Incidensek és &** \> **riasztások**. Vagy közvetlenül a Riasztások **lapra** való ugráshoz használja a <https://security.microsoft.com/alerts> következőt: .
2. Az értesítésre kattintva megjeleníthet egy figyelmeztető lapot, amely információkat tartalmaz az értesítésről.

A riasztásokkal kapcsolatos lépéseket el tudja távolítani, például el kell [távolítania egy gyanús beérkezett üzenetekre vonatkozó szabályt.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Vagy egyszerűen zárja be a  riasztást az értesítési lapon a Feloldás gombra kattintva.

A riasztási házirendek konfigurálásával és kezelésével kapcsolatos további tudnivalók ebben [a cikkben olvashatók.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Fontos:** A Microsoft e-mail-értesítésekkel kapcsolatos értesítései soha nem kérik az alábbiakra:

- Jelszó megadása
- A fiók biztonsági részleteinek ellenőrzése
- Saját hitelesítés újra

Ha ilyen típusú kérésekkel kap e-mailt, azt a Microsoft nem küldte el, és adathalász üzenetnek minősül. Ha ilyen típusú kérésekkel kapcsolatos üzenetet kap, [jelentse az üzenetet a Microsoftnak.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)
