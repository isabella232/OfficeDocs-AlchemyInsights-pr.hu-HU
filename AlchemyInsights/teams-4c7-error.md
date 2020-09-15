---
title: A Teams 4c7 hibaüzenetet kapja hibája
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700205"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 hibaüzenetet kapja hiba a Microsoft Teams alkalmazásban

Ez a hiba azért fordul elő, mert a Microsoft Teams űrlap-hitelesítést követel meg. Ha telepíti az Active Directory összevonási szolgáltatásokat (AD FS), az űrlapos hitelesítés alapértelmezés szerint nincs engedélyezve az intraneten. Ha a Windows beépített hitelesítése nem sikerült, a rendszer az űrlapos hitelesítéssel kéri a bejelentkezést.

A probléma megoldásához engedélyezze az űrlap-hitelesítést az AD FS Microsoft Management Console (MMC) beépülő modullal, amelyen az Active Directory helyi példánya található. Ehhez hajtsa végre a következő lépéseket: 

1. A navigációs ablakban tallózással keresse meg a **hitelesítési szabályokat**.
2. A részletek ablaktábla **műveletek** csoportjában válassza a **globális elsődleges hitelesítés szerkesztése**lehetőséget.
3. Az **intranet** lapon válassza az **űrlapos hitelesítés**lehetőséget.
4. Kattintson **az OK gombra** (vagy az **alkalmaz**gombra).