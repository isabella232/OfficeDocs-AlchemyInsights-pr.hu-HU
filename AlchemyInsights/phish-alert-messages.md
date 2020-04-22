---
title: 2491 E-mail üzenetek riasztása a "Bérlő vagy felhasználó által felülbírálása miatt kézbesített adatlopó" házirendből
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758930"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mail üzenetek riasztása a "Bérlő vagy felhasználó felülbírálása miatt kézbesített adatlopó" házirendből

A "Bérlő vagy felhasználó felülbírálása miatt kézbesített adatphish" nevű alapértelmezett riasztási szabályzat ot vezették be az Office 365 ATP P1 és P2 licenccel rendelkező bérlők számára. Ha ezt a riasztást kapta, az alábbi lépéseket kell kivizsgálnia:

1. A figyelmeztető üzenetben kattintson a **Riasztás megtekintése** gombra a Biztonsági & megfelelőségi központ **Riasztások** lapjára.

2. Válassza ki a riasztást az **üzenetlista** megtekintéséhez vagy az Üzenetek megtekintése az **Intézőben**lehetőséghez. Mindkét lehetőség az üzenet részleteit tartalmazza, beleértve az üzenetazonosítót is. Vegye figyelembe, hogy a Fenyegetéskezelő hivatkozás automatikusan szűri a riasztási feltételeknek megfelelő üzeneteket. Előfordulhat, hogy módosítania kell a dátumszűrőt a Fenyegetéskezelőben.

Az adathalász üzenetet manuálisan konfigurált felülbírálás miatt kézbesítették:

- A felhasználó által beállított engedélyezett feladó vagy tartomány.

- A rendszergazda által a levélszemét elleni házirendben beállított engedélyezett feladó vagy tartomány.

- Engedélyezett IP-cím egy kapcsolatszűrő-házirendben.

- Olyan levélforgalom-szabály (más néven átviteli szabály), amely úgy van beállítva, hogy engedélyezze az üzeneteket.

Ha úgy gondolja, hogy az üzenetet helytelenül jelölték meg adatlopóként, az Outlook [Jelentésüzenet bővítmény segítségével](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) küldjön üzenetmintákat a Microsoftnak.
