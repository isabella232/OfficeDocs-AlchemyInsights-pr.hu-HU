---
title: '2491: E-mailek értesítése a "Kézbesítésről bérlő vagy felhasználó felülbírálása miatt" házirendről'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316360"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mailek riasztása a "Kézbesítés a bérlő vagy a felhasználó felülbírálása miatt" házirendből

A Bérlői  vagy felhasználói felülbírálás miatt a Microsoft DefenderT használó szervezetek a P1 és a P2 licenc esetén Office 365 riasztási házirendet érhetők el. Ha megkapta ezt a riasztást, az alábbi lépéseket követve vizsgálja meg az vizsgálatot:

1. A riasztási üzenetben kattintson az Értesítés megtekintése elemre a riasztások **lapjának** a Microsoft 365 Defender megtekintéséhez. 

2. A figyelmeztetést választva megtekintheti az Üzenetlista megtekintése **vagy** az **Üzenetek megtekintése Intézőben lehetőséget.** Mindkét lehetőséggel az üzenet részleteire megjelenik, amely tartalmazza az üzenetazonosítót. Vegye figyelembe, hogy a Veszélyforrás-intéző hivatkozás automatikusan szűri a riasztási feltételeknek megfelelő üzeneteket. Előfordulhat, hogy módosítania kell a dátumszűrőt a Veszélyforrás-intézőben.

Az adathalász üzenet kézbesítése egy kézzel konfigurált felülbírálás miatt történt:

- A felhasználó által beállított engedélyezett feladó vagy tartomány.
- A rendszergazda által egy levélszemét elleni házirendben beállított engedélyezett feladó vagy tartomány.
- Egy kapcsolatszűrő házirendben engedélyezett IP-cím.
- Egy olyan e-mail-forgalom szabály (más néven átviteli szabály), amely az üzenetek fogadására van beállítva.

Ha úgy véli, hogy az üzenetet [](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) tévesen adathalász üzenetként jelölte meg, a rendszergazdai beküldés segítségével jelentse be az üzenetet a Microsoftnak.

A felhasználók a [Jelentésüzenet](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) vagy az Adathalászat bejelentése bővítmény használatával Outlook mintaüzeneteket küldhetnek a Microsoftnak.
