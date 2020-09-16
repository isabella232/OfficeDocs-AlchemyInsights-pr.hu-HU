---
title: az 2491 riasztási e-mail-üzeneteket a bérlői fiók vagy a felhasználó felülírása házirend szerint
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728613"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mail-üzenetek küldése a bérlői fiók vagy a felhasználó felülírása házirend által kiszállított adathalászó számára

A bérlői fiók vagy a felhasználó felülírása "az adathalászók számára kiszállítva" nevű alapértelmezett riasztási házirendet a bérlők az ATP P1 és 365 a P2 licenccel rendelkező bérlői fiókba építették. Ha ezt az értesítést kapta, az alábbi lépéseket követve vizsgálja meg:

1. A riasztási üzenetben az értesítés **megtekintése** gombra kattintva nyissa meg az **értesítések** lapot a biztonsági & megfelelőségi központban.

2. A riasztás elemre koppintva megtekintheti az **üzenetlistában megtekinthető** és az **üzenetek megtekintése az Intézőben**című témakört. Mindkét beállítással megadhatja az üzenet részleteit, beleértve az üzenet AZONOSÍTÓját is. Fontos tudni, hogy a fenyegetések Explorer hivatkozása automatikusan szűri az értesítési feltételnek megfelelő üzeneteket. Előfordulhat, hogy módosítania kell a szűrőt a fenyegetések Explorerben.

Az adathalászati üzenet a manuálisan konfigurált felülbírálás miatt lett kézbesítve:

- A felhasználó által beállított engedélyezett feladó vagy tartomány.

- Egy levélszemét elleni házirendben a rendszergazda által beállított engedélyezett feladó vagy tartomány.

- Egy engedélyezett IP-cím a kapcsolati szűrő házirendjében.

- E-mail-forgalom szabálya (más néven átviteli szabály), amely az üzenetek engedélyezésére van konfigurálva.

Ha úgy véli, hogy az üzenet tévesen volt megjelölve adathalászként, az Outlook [-jelentés üzenet bővítményével](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) elküldheti az üzenet mintáit a Microsoftnak.
