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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544580"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mail üzenetek riasztása a "Kézbesítés a bérlő vagy a felhasználó felülbírálása miatt" házirendből

A Microsoft Defender Office 365 P1 és P2 licenccel rendelkező bérlői fiókokban egy alapértelmezett "Kézbesítés bérlői fiók vagy felhasználói felülbírálás miatt" nevű riasztási házirendet hoztunk létre. Ha megkapta ezt a riasztást, az alábbi lépéseket kell vizsgálnia:

1. A riasztási üzenetben kattintson a  Riasztás megtekintése elemre a Biztonsági megfelelőségi központ Riasztások & lapjára való ugráshoz. 

2. A figyelmeztetést választva megtekintheti az Üzenetlista megtekintése **vagy** az **Üzenetek megtekintése Intézőben lehetőséget.** Mindkét lehetőséggel az üzenet részleteire megjelenik, amely tartalmazza az üzenetazonosítót. Vegye figyelembe, hogy a Veszélyforrás-intéző hivatkozás automatikusan szűri a riasztási feltételeknek megfelelő üzeneteket. Előfordulhat, hogy módosítania kell a dátumszűrőt a Veszélyforrás-intézőben.

Az adathalász üzenet kézbesítése egy kézzel konfigurált felülbírálás miatt történt:

- A felhasználó által beállított engedélyezett feladó vagy tartomány.

- A rendszergazda által egy levélszemét elleni házirendben beállított engedélyezett feladó vagy tartomány.

- Egy kapcsolatszűrő házirendben engedélyezett IP-cím.

- Egy olyan e-mail-forgalom szabály (más néven átviteli szabály), amely az üzenetek fogadására van beállítva.

Ha úgy véli, hogy az üzenetet helytelenül jelölte [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) meg phish Outlook, az "Üzenet bejelentése" bővítmény használatával küldje el az üzenetmintákat a Microsoftnak.
